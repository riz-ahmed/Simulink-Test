# Simulink-Test
Test cases, execution, reports generation, traceability using Simulink Test

## Test File in Test Manager
Contains multiple test suites and each suite contains multiple test casses

## Baseline test

In baseline test, tests are conducted to assert that the model matches all the requirements that are given in terms of baseline data
One reason to run a baseline test is for regression testing, to see whether the model output still matches the baseline.

There are two tests:
- The first test verifies whether a model meets a requirement.
- The second test compares a simulation result to baseline data.

### Test Harness
Using test harness, isolates the test object from its environment as well as it interactions form other components so that the test object can be tested in isolation.
The required signals for the test object are then supplied as simulated signals and the outputs are measured using sinks such as scope blocks. By isolating a test object using test harness, un-necessary verification and asssessment blocks that you don't want in the main model. Using test harness, unit-test on conroller can be done. It is also possible to isolate the whole system into test harness and perform system level tests.

Once the test manager reports test fail and highlights the model where the assertion failure has occured, the test object is isolated into a test harness model for more detailed analysis and further test case executions

### Creating a test harness in simulink
In simulink, test harness is created by selecting the controller logic sub-system and adding it to "create test harness" (option after right-click on simulink sub-system block). Create inputs such as constants or using signal builder (as well as external data files) and scopes for observing the output from the controller logic.

Once the test harness is created, testing can be done by simulating the test harness model. 
