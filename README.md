# AndroidSensors
iin this workshop we will do with Sensors in Android Appp 

## Steps1:List of sensors
create a composable that displays a list of sensors
1.declare and instantiate a sensor mamager 
```kotlin
  val context = LocalContext.current
   val sensorManager = context.getSystemService<SensorManager>()```
acceder à la liste des capteurs 
```kotlin
    val deviceSensors= sensorManager?.getSensorList(Sensor.TYPE_ALL) as List<Sensor>;
```
display name and type in LazyColumn
## Step2: Temperature Sensor  
1. register listener for temperature listener in start method
2. stop in the stop method
3. implement  override fun onSensorChanged(p0: SensorEvent?)
4. Test application
