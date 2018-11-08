# Examples

These are two examples programs that require the library to be built before 
they can be run. These are adapted from the tests for the BN254CX curve.
Replace `VERSION` below with required version.

    javac -classpath .:../build/libs/milagro-crypto-java-VERSION.jar  TestMPIN.java
    java -classpath .:../build/libs/milagro-crypto-java-VERSION.jar  TestMPIN

    javac -classpath .:../build/libs/milagro-crypto-java-VERSION.jar  TestECC.java
    java -classpath .:../build/libs/milagro-crypto-java-VERSION.jar  TestECC
