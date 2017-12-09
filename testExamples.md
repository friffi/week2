# Test Examples

### Scenario: Illegal move 

##### Given: [GameCreated(), GameJoined(), Placed(0,0,X)]

##### When: Place(0,0,O)

##### Then: [IllegalMove] // Move has already been made

### Scenario: Illegal move 

##### Given: [GameCreated(), GameJoined(), Placed(1,1,X)]

##### When: Place(1,2,X)

##### Then: [IllegalMove] // Not your turn



### Scenario: X wins

##### Given: [GameCreated(), GameJoined(), Placed(0,0,X), Placed(1,0,O), Placed(0,1,X), Placed(2,0,O)]

##### When: Place(0,2,X)

##### Then: [Place(0,2,X), X Won]

### Scenario: X wins

##### Given: [GameCreated(), GameJoined(), Placed(0,0,X), Placed(0,1,O), Placed(1,1,X), Placed(2,0,O)]

##### When: Place(2,2,X)

##### Then: [Place(2,2,X), X Won]

### Scenario: O wins

##### Given: [GameCreated(), GameJoined(), Placed(1,1,X), Placed(0,0,O), Placed(1,2,X), Placed(1,0,O), Placed(1,2,X)]

##### When: Place(2,0,O)

##### Then: [Place(2,0,O), O Won]


### Scenario: Draw

##### Given: [GameCreated(), GameJoined(), Placed(0,0,X), Placed(0,1,O), Placed(0,2,X), Placed(1,0,O), Placed(1,1,X), Placed(2,0,O), Placed(1,2,X), Placed(2,2,0)]

##### When: Place(2,1,X)

##### Then: [Place(2,1,X), Draw]

### Scenario: Draw

##### Given: [GameCreated(), GameJoined(), Placed(0,1,X), Placed(0,0,0), Placed(0,2,X), Placed(1,1,O), Placed(1,0,X), Placed(1,2,O), Placed(2,1,X), Placed(2,0,O)]

##### When: Place(2,2,X)

##### Then: [Place(2,2,X), Draw]



