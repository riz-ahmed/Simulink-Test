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
The required signals for the test object are then supplied as simulated signals.

Once the test manager reports test fail and highlights the model where the assertion failure has occured, the test object is isolated into a test harness model for more detailed analysis and further test case executions

