# mse-isobmff-bsf-tests
Repository for testing support of ISOBMFF MSE Byte Stream Format

The file tests.json provides a JSON array of test objects with the following properties:
- "name" string corresponding to the name of the test file
-	"valid": boolean indicating if the test is meant to be valid against current spec
- "description": short description of the test file 
- "reason": short explaining of why it would be invalid if valid = false
- "passed": a JSON object containing 3 properties ("Chrome", "Firefox", "Safari") with the following syntax: true if the test passes (i.e. no error if valid; throwing error if invalid), false if the test does not pass (error if valid; no error if invalid) or a String corresponding to the error message reported in the inspector
