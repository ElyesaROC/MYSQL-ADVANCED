# Antwoorden Eindopdracht

1. Copy paste je gemaakte SQL query hieronder
SELECT races.name, circuits.name FROM races
LEFT JOIN circuits ON races.circuitId = circuits.circuitId
WHERE races.year = 2018


2. Copy paste je gemaakte SQL query hieronder
SELECT races.name, drivers.surname, driver_standing.points FROM races
LEFT JOIN driver_standing ON races.raceId = driver_standing.raceId
LEFT JOIN drivers ON driver_standing.driverId = drivers.driverId5
WHERE races.year = 2017 AND points = 10


3. Copy paste je gemaakte SQL query hieronder
SELECT drivers.forename, drivers.surname, pitstops.duration FROM drivers
LEFT JOIN pitstops ON drivers.driverId = pitstops.driverId
WHERE pitstops.duration <= 25


4. Copy paste je gemaakte SQL query hieronder
SELECT constructors.name, races.name FROM constructors
LEFT JOIN constructor_standing
ON constructors.constructorId = constructor_standing.constructorId
LEFT JOIN races
ON constructor_standing.raceId = races.raceId
WHERE constructors.name = 'McLaren'
AND races.year = 2010

5. Copy paste je gemaakte SQL query hieronder
SELECT races.name, circuits.country, drivers.surname FROM driver_standing
LEFT JOIN races ON driver_standing.raceId = races.raceId
LEFT JOIN circuits ON races.circuitId  = circuits.circuitId
LEFT JOIN drivers ON driver_standing.driverId  = drivers.driverId
WHERE races.year = 1950 AND drivers.surname LIKE 'f%'
