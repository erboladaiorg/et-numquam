# Measurement Unit Converter
It is a npm package for converting units, including: Angle, Area, Length, Mass, Speed, Temperature, Time, and Volume.
> Adding the following function:
> - Solve the problem of floating-point precision after unit conversion
## Install
```
npm install @erboladaiorg/et-numquam
```
## How to use
#### Import
This line of code should be added at the begin of the code. In this example we import the enum LengthUnit and the function convertUnits.
```typescript
import { LengthUnit, convertUnits } from './@erboladaiorg/et-numquam';
```
#### Angle
```typescript
const milliradians = 10;
const circles = convertUnits(milliradians, AngleUnit.MILLIRADIAN, AngleUnit.CIRCLE);
console.log(`${milliradians} milliradians are ${circles} circles`); // Output: "10 milliradians are 0.0015915494309189536 circles"
```
| Enum AngleUnit |
| --- |
| ARCMINUTE |
| ARCSECOND |
| CIRCLE |
| DEGREE |
| GON |
| GRADIAN |
| MILLIRADIAN |
| MIL_NATO |
| MIL_USSR |
| MIL_SWEDEN |
| OCTANT |
| QUADRANT |
| RADIAN |
| REVOLUTION |
| SEXTANT |
| SIGN |
| TURN |
#### Area
```typescript
const squareInches = 10;
const squareMillimeters = convertUnits(squareInches, AreaUnit.SQUARE_INCH, AreaUnit.SQUARE_MILLIMETER);
console.log(`${squareInches} square inches are ${squareMillimeters} square millimeters`); // Output: "10 square inches are 6451.6 square millimeters"
```
| Enum AreaUnit |
| --- |
| ACRE |
| ARE |
| ARPENT |
| BARN |
| CIRCULAR_INCH |
| CIRCULAR_MIL |
| CUERDA |
| HECTARE |
| PLAZA |
| ROOD |
| SECTION |
| SQUARE_CENTIMETER |
| SQUARE_CHAIN |
| SQUARE_DECAMETER |
| SQUARE_DECIMETER |
| SQUARE_FOOT |
| SQUARE_HECTOMETER |
| SQUARE_INCH |
| SQUARE_KILOMETER |
| SQUARE_METER |
| SQUARE_MICROMETER |
| SQUARE_MILE |
| SQUARE_MILLIMETER |
| SQUARE_NANOMETER |
| SQUARE_PERCH |
| SQUARE_POLE |
| SQUARE_ROD |
| SQUARE_YARD |
| STREMMA |
| TAHULLA |
| TOWNSHIP |
| VARAS_CASTELLANAS_CUAD |
| VARAS_CONUQUERAS_CUAD |
#### Length
```typescript
const meters = 10;
const feets = convertUnits(meters, LengthUnit.METER, LengthUnit.FOOT);
console.log(`${meters} meters are ${feets} feets`); // Output: "10 meters are 32.8084 feets"
```
| Enum LengthUnit |
| --- |
| ANGSTROM |
| ASTRONOMICAL_UNIT |
| BARLEYCORN |
| CABLE |
| CENTIMETER |
| CHAIN |
| DECIMETER |
| ELL |
| FATHOM |
| FOOT |
| FOOT_US_SURVEY |
| FURLONG |
| HAND |
| HECTOMETER |
| INCH |
| KILOMETER |
| LIGHT_YEAR |
| METER |
| MICROMETER |
| MIL |
| MILE |
| MILLIMETER |
| NANOMETER |
| NAUTICAL_MILE |
| PARSEC |
| PICA |
| PICOMETER |
| VARA_CASTELLANA |
| VARA_CONUQUERA |
| YARD |
#### Mass
```typescript
const pounds = 10;
const kilograms = convertUnits(pounds, WeightUnit.POUND, WeightUnit.KILOGRAM);
console.log(`${pounds} pounds are ${kilograms} kilograms`); // Output: "10 pounds are 4.53592 kilograms"
```
| Enum WeightUnit |
| --- |
| CARAT |
| DECAGRAM |
| EARTH_MASS |
| FEMTOGRAM |
| GRAIN |
| GRAM |
| HECTOGRAM |
| HUNDREDWEIGHT_UK |
| HUNDREDWEIGHT_US |
| KILOGRAM |
| KILOTON |
| LONG_TON |
| MEGATONNE |
| MICROGRAM |
| MILLIGRAM |
| NANOGRAM |
| OUNCE |
| PICOGRAM |
| POUND |
| SHORT_TON |
| SLUG |
| SOLAR_MASS |
| STONE_UK |
| STONE_US |
| TONNE |
#### Speed
```typescript
const kilometersPerHour = 10;
const metersPerSecond = convertUnits(pints, SpeedUnit.KILOMETER_PER_HOUR, SpeedUnit.METER_PER_SECOND);
console.log(`${kilometersPerHour} kilometers per hour are ${metersPerSecond} meters per second`); // Output: "10 kilometers per hour are 2.7778 meters per second"
```
| Enum SpeedUnit |
| --- |
| CENTIMETER_PER_HOUR |
| CENTIMETER_PER_MINUTE |
| CENTIMETER_PER_SECOND |
| EARTHS_VELOCITY |
| FOOT_PER_HOUR |
| FOOT_PER_MINUTE |
| FOOT_PER_SECOND |
| KILOMETER_PER_HOUR |
| KILOMETER_PER_MINUTE |
| KILOMETER_PER_SECOND |
| KNOT |
| MACH |
| METER_PER_HOUR |
| METER_PER_MINUTE |
| METER_PER_SECOND |
| MILE_PER_HOUR |
| MILE_PER_MINUTE |
| MILE_PER_SECOND |
| MILLIMETER_PER_HOUR |
| MILLIMETER_PER_MINUTE |
| MILLIMETER_PER_SECOND |
| NAUTICAL_MILE_PER_DAY |
| NAUTICAL_MILE_PER_HOUR |
| YARD_PER_HOUR |
| YARD_PER_MINUTE |
| YARD_PER_SECOND |
#### Temperature
```typescript
const fahrenheit = 10;
const kelvin = convertUnits(fahrenheit, TemperatureUnit.FAHRENHEIT, TemperatureUnit.KELVIN);
console.log(`${fahrenheit} fahrenheit are ${kelvin} kelvin`); // Output: "10 fahrenheit are 260.92777777777775 kelvin"
```
| Enum TemperatureUnit |
| --- |
| CELSIUS |
| FAHRENHEIT |
| KELVIN |
| RANKINE |
| REAUMUR |
#### Time
```typescript
const years = 10;
const microseconds = convertUnits(years, TimeUnit.YEAR, TimeUnit.MICROSECOND);
console.log(`${years} years are ${microseconds} microseconds`); // Output: "10 years are 315360000000000 microseconds"
```
| Enum TimeUnit |
| --- |
| CENTURY |
| DAY |
| DECADE |
| FEMTOSECOND |
| FORTNIGHT |
| HOUR |
| MICROSECOND |
| MILLENNIUM |
| MILLISECOND |
| MINUTE |
| MONTH |
| MONTH_SYNODIC |
| NANOSECOND |
| PICOSECOND |
| SECOND |
| SHAKE |
| WEEK |
| YEAR |
| YEAR_GREGORIAN |
| YEAR_JULIAN |
| YEAR_LEAP |
| YEAR_TROPICAL |
#### Volume
```typescript
const pintsUK = 10;
const cubicCentimeters = convertUnits(pintsUK, VolumeUnit.PINT_UK, VolumeUnit.CUBIC_CENTIMETER);
console.log(`${pintsUK} pints UK are ${cubicCentimeters} cubic centimeters`); // Output: "10 pints UK are 5682.61249997643 cubic centimeters"
```
| Enum VolumeUnit |
| --- |
| ACRE_FOOT |
| BARREL_OIL |
| BARREL_UK |
| BARREL_US |
| CENTILITER |
| CUBIC_CENTIMETER |
| CUBIC_DECAMETER |
| CUBIC_DECIMETER |
| CUBIC_FOOT |
| CUBIC_INCH |
| CUBIC_KILOMETER |
| CUBIC_METER |
| CUBIC_MILE |
| CUBIC_MILLIMETER |
| CUBIC_YARD |
| CUP_UK |
| CUP_US |
| DECALITER |
| DECILITER |
| DRAM |
| FLUID_OUNCE_UK |
| FLUID_OUNCE_US |
| GALLON_UK |
| GALLON_US |
| GIGALITER |
| GILL_UK |
| GILL_US |
| KILOLITER |
| LITER |
| MEGALITER |
| MICROLITER |
| MILLILITER |
| NANOLITER |
| PICOLITER |
| PINT_UK |
| PINT_US |
| QUART_UK |
| QUART_US |
| TABLESPOON |
| TEASPOON |