# Advanced mockito
## Arguments Matcher
Used to perform conditional returns if the argument passed to a mocked object matches some condition. See also Answers to more complex tests.
### Structure
`given( mock.method( argThat( argument -> <condition>))).willReturn(object)`
### See more
https://www.baeldung.com/mockito-argument-matchers

## Argument Capture
Used to perform return one or other object depending of the argument captured in the mocked object.
### Structure
`given( mock.method( captor.capture()).willReturn(object)`

## Answers
Used to return certain object depending of the argument passed previously.
### Structure
`given( mock.method( captor.capture()).willAnswer( invocation -> <condition_on_captured>)`

## Mock
A mock is simply an object for test that does not have actual implementation and only serve to stub method invocations.

## Spy
An spy is simply a mocked object that has its own implementation and can change with method calls, so the invocations over its own methods change the state of the object.
### See more
https://www.baeldung.com/mockito-spy

### Examples
<script src="https://gist.github.com/PabloVillacanhas/73de599d9ae77db8df6714998d80ea51.js"></script>

---
## Further References:
https://www.udemy.com/course/testing-spring-boot-beginner-to-guru

