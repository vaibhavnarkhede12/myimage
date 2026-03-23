
    # Access the list of earthquakes
    events = data["features"]

    # 1. TotalEvents: How many quakes are there in total?
    TotalEvents = len(events)

    # 2. TotalFelt: How many quakes were felt by at least 100 people?
    # We use filter() to find events where 'felt' is not None and >= 100
    felt_100_plus = list(filter(lambda x: x["properties"]["felt"] is not None and x["properties"]["felt"] >= 100, events))
    TotalFelt = len(felt_100_plus)

    # 3. MostFeltEvent & MostFeltCount
    # Use max() with a key to find the event with the highest 'felt' value
    # We use .get("felt") or 0 to handle cases where 'felt' might be null/None
    most_felt_obj = max(events, key=lambda x: x["properties"]["felt"] if x["properties"]["felt"] is not None else 0)
    
    MostFeltEvent = most_felt_obj["properties"]["title"]
    MostFeltCount = most_felt_obj["properties"]["felt"]
