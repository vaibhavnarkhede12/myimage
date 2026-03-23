    # 1. Create an empty dictionary to hold the counts
    event_counts = {}

    # 2. Iterate through the features in the JSON data
    for feature in data["features"]:
        # Get the event type (e.g., 'earthquake', 'quarry blast')
        event_type = feature["properties"]["type"]
        
        # 3. Update the count in the dictionary
        if event_type in event_counts:
            event_counts[event_type] += 1
        else:
            event_counts[event_type] = 1

    # 4. Return the resulting dictionary
    return event_counts
