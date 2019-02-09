def calculate_distance_in_km(volume_in_litres, fuel_consump):

    """
    >>> calculate_distance_in_km(60,8)
    750.0

    >>> calculate_distance_in_km(60,8)
    700.0

    :param volume_in_litres:
    :param fuel_consump:
    :return:
    """

    distance = volume_in_litres / fuel_consump * 100
    return distance

print(calculate_distance_in_km(60, 8))
# print(calculate_distance_in_km(45, 8))
# print(calculate_distance_in_km(30, 8))
# print(calculate_distance_in_km(15, 8))

