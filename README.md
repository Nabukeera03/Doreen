def sum_timestamps(timestamps):
    total_seconds = 0

    for timestamp in timestamps:
        minutes,seconds = timestamp.split(":")
        total_seconds += int(minutes) * 60 + int(seconds)

    minutes, seconds = divmod(total_seconds, 60)
    return f"{minutes:02d}:{seconds:02d}"
    

timestamps = ["1:00", "2:00", "4:00"]
result = sum_timestamps(timestamps)
print(result)

sum_timestamps(timestamps0)