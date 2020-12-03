# Get table definitions in WebFOCUS

If you need to know what the data types of a `TABLE FILE` in WebFOCUS are, you can enter the command:

```
?FF {TABLE_NAME}
```

## Usage

```
?FF CAR
```

returns

```
 FILENAME=  CAR
 COUNTRY       COUNTRY       A10
 CAR           CARS          A16
 MODEL         MODEL         A24
 BODYTYPE      TYPE          A12
 SEATS         SEAT          I3
 DEALER_COST   DCOST         D7
 RETAIL_COST   RCOST         D7
 SALES         UNITS         I6
 LENGTH        LEN           D5
 WIDTH         WIDTH         D5
 HEIGHT        HEIGHT        D5
 WEIGHT        WEIGHT        D6
 WHEELBASE     BASE          D6.1
 FUEL_CAP      FUEL          D6.1
 BHP           POWER         D6
 RPM           RPM           I5
 MPG           MILES         D6
 ACCEL         SECONDS       D6
 WARRANTY      WARR          A40
 STANDARD      EQUIP         A40
```
