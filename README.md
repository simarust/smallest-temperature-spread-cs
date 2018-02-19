# MinTempSpread

## Description
This is a C# console application discovering the smallest temperature spread from a weather data file.

## Program.cs [(show)](MinTempSpread/Program.cs)
- (Program.cs)[MinTempSpread/Program.cs]
- Reads the data file
- Calls a factory method to get a list of TemperatureData objects
- Orders the list ascending by temperature difference and takes the first entry of that list to get the entry smallest temperature spread.

## TemperatureData.cs [(show)](MinTempSpread/TemperatureData.cs)
- Provides a 'factory' method to create a list of objects containing the day and the highest and lowest temperature of each day.
- Parses the provided raw data line by line using a regex containing groups.
- Returns a list of TemperatureData objects
