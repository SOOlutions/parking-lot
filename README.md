# parking-lot
Design a parking lot using object-oriented principles?

# Requirements

1. The parking lot has multiple levels. Each level has multiple rows of spots.

2. The parking lot can park motorcycles, cars, and buses.

3. The parking lot has motorcycle spots, compact spots, and large spots.

4. A motorcycle can park in any spot.

5. A car can park in either a single compact spot or a single large spot.

6. A bus can park in five large spots that are consecutive and within the same row. It cannot park in small spots.

# Stories

_For Behavior Driven Development purpose_

## Feature: car

> In order to park my car
> As a driver
> I need to be able to see if there is a spot left

### Scenario 1:

 - **Given** I am in front of the entrance
 - **And** I'm driving a car
 - **And** There is 10 compact spots left
 - **And** There is 2 large spots left
 - **When** I read the information panel
 - **Then** I should see a line displaying "cars: 10 spots"
 - **And** I have access to the ticket machine

### Scenario 2:

 - **Given** I am in front of the entrance
 - **And** I'm driving a car
 - **And** There is no compact spots left
 - **And** There is no large spot left
 - **When** I read the information panel
 - **Then** I should see a line displaying "cars: full"
 - **And** I cannot access the ticket machine

[...]
