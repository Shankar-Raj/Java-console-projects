# Bus Timings Console Application

This is a simple Java console application that helps users manage and search for bus timings without requiring a map interface. The application offers two main functionalities:

1. **Add/Update Bus Information**  
2. **Search Bus Timings**

## 1. Add/Update Interface

### 1.1. Add Bus Details  
Users can add new bus information by providing the following details:
- **Bus Number**
- **Bus Stop(s)**
- **Bus Timing(s)**

### 1.2. Update Bus Details  
Users can update existing bus information in three different ways:
- **Update Bus Number**: Modify the bus number for an existing bus route.
- **Update Stopping**: Change the bus stops on an existing route.
- **Update Timings**: Adjust the timings for a specific bus route.

## 2. Search Interface

### 2.1. Search by Bus Number  
Allows users to search for the timings of a particular bus by entering the bus number.

### 2.2. Search by Place  
Users can search for bus timings by specifying the starting and ending locations. The system will display the bus options and their timings for the route between the two locations.

## Key Features & Benefits

1. **No Map Interface Required**  
   The project functions entirely through a console-based interface, making it simple and easy to use without requiring a map.

2. **Easy Bus Details Management**  
   When adding new bus information, users don't need to manually enter the exact timing for each stop. The application automatically generates a timetable based on bus stops and timings. Just by giving like Stops : A,B,C and Timings: 1,2,3,4,5,6,7,8,9. For example:
   ```
   Stops: A  B  C
   Timings:
   1  2  3
   6  5  4
   7  8  9
   ```

3. **Simplified Timing Calculation**  
   Users don't need to calculate or assign specific timings for each bus stop. The system automatically handles the arrangement and displays it in a clear, tabular format.

4. **Efficient Route Search**  
   Users can easily search for available buses between two points. If no direct bus is available, the system identifies alternate routes and suggests a common stop:
   - **Bus No**: The bus that will take you from point A to the common stop B.
   - **Timings**: Pickup and drop timings for each leg of the journey.

   For example, if traveling from A to C but no direct bus exists, the system will suggest buses that go from A to B and then from B to C.

5. **Full Bus Schedule**  
   Users can view the full schedule of a bus by simply providing the bus number. The application displays the stops and corresponding timings in an easy-to-read format:
   ```
   Bus No: <BusNumber>
   Stops:  A  B  C
   Timings:
   1  2  3
   6  5  4
   7  8  9
   ```

-------------------------------------------------------------------------------------------
# KeypadWords

This Java program converts sequences of keypresses on a traditional mobile keypad into corresponding letters. It interprets the number of times a key is pressed to determine the correct letter.

## Features

- Converts numeric key sequences into words using a traditional mobile keypad layout.
- Handles key inputs including spaces and keys without corresponding letters.

## Keypad Layout

The program recognizes the following key mappings:

- `0`: Space
- `1`: No letters
- `2`: a, b, c
- `3`: d, e, f
- `4`: g, h, i
- `5`: j, k, l
- `6`: m, n, o
- `7`: p, q, r, s
- `8`: t, u, v
- `9`: w, x, y, z

## Usage :

1. Follow the prompts to enter a sequence of keypresses. For example:
   ```
   2 22 3 33
   ```

2. The program will output the corresponding letters based on your input.

## Example

Input: `2 22 3 33`  
Output: `abcde`
