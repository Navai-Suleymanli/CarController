## Car Controller

This script provides basic car control functionality in a Unity game. It allows the player to control a car using keyboard inputs and simulates the movement and audio of a car.

### Features
- Wheel Colliders: Four wheel colliders are attached to the car, representing the front right, front left, back right, and back left wheels.
- Transform Components: Transform components are assigned to the wheel colliders to update their positions and rotations based on physics simulation.
- Acceleration: The car has an acceleration parameter that determines how quickly it can speed up.
- Breaking Force: The car has a breaking force parameter that determines how quickly it can slow down.
- Maximum Turn Angle: The maximum angle the front wheels can turn when steering.
- Audio: The car has an audio source that plays engine sounds with varying volumes based on the car's velocity.

### Usage
1. Attach this script to a car game object in your scene.
2. Assign the appropriate wheel colliders to the serialized fields of the script:
   - `frontRight`: Front right wheel collider.
   - `frontLeft`: Front left wheel collider.
   - `backRight`: Back right wheel collider.
   - `backLeft`: Back left wheel collider.
3. Assign the appropriate transform components to the serialized fields of the script:
   - `frontRightTransform`: Transform component for the front right wheel.
   - `frontLeftTransform`: Transform component for the front left wheel.
   - `backRightTransform`: Transform component for the back right wheel.
   - `backLeftTransform`: Transform component for the back left wheel.
4. Adjust the values of the public parameters (`acceleration`, `breakingForce`, `maxTurnAngle`) to fit your car's behavior.
5. Optionally, assign an audio clip to the `carSound` field to customize the engine sound.
6. Add a Rigidbody component to the car game object if it doesn't have one already.
7. Ensure the player game object is assigned to the `Player` field of the script.
8. Run the game and control the car using the following inputs:
   - Accelerate: Use the vertical axis (usually the W key) to move the car forward.
   - Brake: Use the space bar to apply brakes and slow down the car.
   - Steer: Use the horizontal axis (usually the A and D keys) to steer the car left or right.
   - Enter/Exit Car: When near the car (within a distance of 5 units), press the E key to enter or exit the car.

Note: The script assumes that the player game object has an active state that controls its visibility and interaction.

