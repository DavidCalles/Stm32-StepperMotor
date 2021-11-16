# Stm32-StepperMotorQueue

Using linked lists and interrupts, the user can create isntructions for a steper motor through a commands parser.
Commands will be executed once at a time to move a stepper motor at a given speed for a given number of times.

# Usage

Through a serial terminal type:

    help

To see a lsit of all the commands avaialble.  

    stepperinit

To initialize the timers and hardware needed for the stepper motor quesue functionality.

    stepperenable <1|0>

To enable the configured output of the stepper motor. And finally:

    step2 <NUM_STEPS> <STEP_TIME>

To add a specific number of steps at a given speed to the motor's queue. 
NUM_STEPS can be negative to make the mtoor go in the oposite direction.
