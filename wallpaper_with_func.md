def calculate_wallpaper_amount (room_length_in_metres,
                                room_width_in_metres,
                                wallpaper_width_in_metres,
                                room_height_in_metres,
                                wallpaper_length_in_metres):
    """
    >>> calculate_wallpaper_amount(5,6,1.06,2.75,10)
    7.0

    >>> calculate_wallpaper_amount(5,6,1.06,2.75,10)
    8.0

    :param room_length_in_metres:
    :param room_width_in_metres:
    :param wallpaper_width_in_metres:
    :param room_height_in_metres:
    :param wallpaper_length_in_metres:
    :return:
    """

    perimeter = (room_length_in_metres + room_width_in_metres) * 2
    stripes_amount = round(perimeter / wallpaper_width_in_metres)
    stripes_in_roll_amount = int(wallpaper_length_in_metres / (room_height_in_metres + 0.1))
    roll_amount = stripes_amount / stripes_in_roll_amount
    return roll_amount

print (calculate_wallpaper_amount(5,6, 1.06, 2.75, 10))
