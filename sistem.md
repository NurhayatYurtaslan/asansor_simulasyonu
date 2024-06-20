| Class            | Attributes                       | Methods                | Relations                          | Notes                              |
|------------------|----------------------------------|------------------------|------------------------------------|------------------------------------|
| Building         | - numFloors: int                  | + requestElevator     | - elevators: List of Elevator      |                                    |
|                  | - elevators: List of Elevator     | + registerArrival     |                                    |                                    |
|                  | - floors: List of Floor           | + update()            |                                    |                                    |
| Elevator         | - elevatorID: int                 | + moveToFloor         | - controlPanel: ControlPanel       |                                    |
|                  | - currentFloor: int               | + openDoors()         |                                    |                                    |
|                  | - capacity: int                   | + closeDoors()        |                                    |                                    |
|                  | - doorsOpen: boolean              |                        |                                    |                                    |
|                  | - direction: Direction            |                        |                                    |                                    |
| Floor            | - floorNum: int                   |                        | - callButtons: List of CallButton  |                                    |
|                  | - callButtons: List of CallButton |                        | - arrivalIndicators: List of       |                                    |
|                  | - arrivalIndicators: List of      |                        |   ArrivalIndicator                 |                                    |
|                  |   ArrivalIndicator                |                        |                                    |                                    |
| ControlPanel     | - destinationButtons: List of     |                        |                                    |                                    |
|                  |   Button                          |                        |                                    |                                    |
|                  | - emergencyButton: Button         |                        |                                    |                                    |
| CallButton       | - direction: Direction            |                        |                                    |                                    |
| ArrivalIndicator | - direction: Direction            |                        |                                    |                                    |
|                  | - lightOn: boolean                |                        |                                    |                                    |
| Button           | - isPressed: boolean              |                        |                                    |                                    |
