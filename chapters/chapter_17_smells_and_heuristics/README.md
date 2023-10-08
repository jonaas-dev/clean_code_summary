<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [CHAPTER 17: SMELLS AND HEURISTICS](#chapter-17-smells-and-heuristics)
  - [Comments](#comments)
    - [C1: Inappropriate Information](#c1-inappropriate-information)
    - [C2: Obsolete Comment](#c2-obsolete-comment)
    - [C3: Redundant Comment](#c3-redundant-comment)
    - [C4: Poorly Written Comment](#c4-poorly-written-comment)
    - [C5: Commented-Out Code](#c5-commented-out-code)
  - [Environment](#environment)
    - [E1: Build Requires More Than One Step](#e1-build-requires-more-than-one-step)
    - [E2: Tests Require More Than One Step](#e2-tests-require-more-than-one-step)
  - [Functions](#functions)
    - [F1: Too Many Arguments](#f1-too-many-arguments)
    - [F2: Output Arguments](#f2-output-arguments)
    - [F3: Flag Arguments](#f3-flag-arguments)
    - [F4: Dead Function](#f4-dead-function)
  - [General](#general)
    - [G1: Multiple Languages in One Source File](#g1-multiple-languages-in-one-source-file)
    - [G2: Obvious Behavior Is Unimplemented](#g2-obvious-behavior-is-unimplemented)
    - [G3: Incorrect Behavior at the Boundaries](#g3-incorrect-behavior-at-the-boundaries)
    - [G4: Overridden Safeties](#g4-overridden-safeties)
    - [G5: Duplication](#g5-duplication)
    - [G6: Code at Wrong Level of Abstraction](#g6-code-at-wrong-level-of-abstraction)
    - [G7: Base Classes Depending on Their Derivatives](#g7-base-classes-depending-on-their-derivatives)
    - [G8: Too Much Information](#g8-too-much-information)
    - [G9: Dead Code](#g9-dead-code)
    - [G10: Vertical Separation](#g10-vertical-separation)
    - [G11: Inconsistency](#g11-inconsistency)
    - [G12: Clutter](#g12-clutter)
    - [G13: Artificial Coupling](#g13-artificial-coupling)
    - [G14: Feature Envy](#g14-feature-envy)
    - [G15: Selector Arguments](#g15-selector-arguments)
    - [G16: Obscured Intent](#g16-obscured-intent)
    - [G17: Misplaced Responsibility](#g17-misplaced-responsibility)
    - [G18: Inappropriate Static](#g18-inappropriate-static)
    - [G19: Use Explanatory Variables](#g19-use-explanatory-variables)
    - [G20: Function Names Should Say What They Do](#g20-function-names-should-say-what-they-do)
    - [G21: Understand the Algorithm](#g21-understand-the-algorithm)
    - [G22: Make Logical Dependencies Physical](#g22-make-logical-dependencies-physical)
    - [G23: Prefer Polymorphism to If/Else or Switch/Case](#g23-prefer-polymorphism-to-ifelse-or-switchcase)
    - [G24: Follow Standard Conventions](#g24-follow-standard-conventions)
    - [G25: Replace Magic Numbers with Named Constants](#g25-replace-magic-numbers-with-named-constants)
    - [G26: Be Precise](#g26-be-precise)
    - [G27: Structure over Convention](#g27-structure-over-convention)
    - [G28: Encapsulate Conditionals](#g28-encapsulate-conditionals)
    - [G29: Avoid Negative Conditionals](#g29-avoid-negative-conditionals)
    - [G30: Functions Should Do One Thing](#g30-functions-should-do-one-thing)
    - [G31: Hidden Temporal Couplings](#g31-hidden-temporal-couplings)
    - [G32: Don’t Be Arbitrary](#g32-dont-be-arbitrary)
    - [G33: Encapsulate Boundary Conditions](#g33-encapsulate-boundary-conditions)
    - [G34: Functions Should Descend Only](#g34-functions-should-descend-only)
  - [One Level of Abstraction](#one-level-of-abstraction)
    - [G35: Keep Configurable Data at High Levels](#g35-keep-configurable-data-at-high-levels)
    - [G36: Avoid Transitive Navigation](#g36-avoid-transitive-navigation)
- [Java](#java)
    - [J1: Avoid Long Import Lists by Using Wildcards](#j1-avoid-long-import-lists-by-using-wildcards)
    - [J2: Don’t Inherit Constants](#j2-dont-inherit-constants)
    - [J3: Constants versus Enums](#j3-constants-versus-enums)
  - [Names](#names)
    - [N1: Choose Descriptive Names](#n1-choose-descriptive-names)
    - [N2: Choose Names at the Appropriate Level of Abstraction](#n2-choose-names-at-the-appropriate-level-of-abstraction)
    - [N3: Use Standard Nomenclature Where Possible](#n3-use-standard-nomenclature-where-possible)
    - [N4: Unambiguous Names](#n4-unambiguous-names)
    - [N5: Use Long Names for Long Scopes](#n5-use-long-names-for-long-scopes)
    - [N6: Avoid Encodings](#n6-avoid-encodings)
    - [N7: Names Should Describe Side-Effects](#n7-names-should-describe-side-effects)
  - [Tests](#tests)
    - [T1: Insufficient Tests](#t1-insufficient-tests)
    - [T2: Use a Coverage Tool!](#t2-use-a-coverage-tool)
    - [T3: Don’t Skip Trivial Tests](#t3-dont-skip-trivial-tests)
    - [T4: An Ignored Test Is a Question about an Ambiguity](#t4-an-ignored-test-is-a-question-about-an-ambiguity)
    - [T5: Test Boundary Conditions](#t5-test-boundary-conditions)
    - [T6: Exhaustively Test Near Bugs](#t6-exhaustively-test-near-bugs)
    - [T7: Patterns of Failure Are Revealing](#t7-patterns-of-failure-are-revealing)
    - [T8: Test Coverage Patterns Can Be Revealing](#t8-test-coverage-patterns-can-be-revealing)
    - [T9: Tests Should Be Fast](#t9-tests-should-be-fast)
  - [Conclusion](#conclusion)
  - [Bibliography](#bibliography)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->





## CHAPTER 17: SMELLS AND HEURISTICS

### Comments
#### C1: Inappropriate Information
#### C2: Obsolete Comment
#### C3: Redundant Comment
#### C4: Poorly Written Comment
#### C5: Commented-Out Code

### Environment
#### E1: Build Requires More Than One Step
#### E2: Tests Require More Than One Step

### Functions
#### F1: Too Many Arguments
#### F2: Output Arguments
#### F3: Flag Arguments
#### F4: Dead Function

### General

#### G1: Multiple Languages in One Source File
#### G2: Obvious Behavior Is Unimplemented
#### G3: Incorrect Behavior at the Boundaries
#### G4: Overridden Safeties
#### G5: Duplication
#### G6: Code at Wrong Level of Abstraction
#### G7: Base Classes Depending on Their Derivatives
#### G8: Too Much Information
#### G9: Dead Code
#### G10: Vertical Separation
#### G11: Inconsistency
#### G12: Clutter
#### G13: Artificial Coupling
#### G14: Feature Envy
#### G15: Selector Arguments
#### G16: Obscured Intent
#### G17: Misplaced Responsibility
#### G18: Inappropriate Static
#### G19: Use Explanatory Variables
#### G20: Function Names Should Say What They Do
#### G21: Understand the Algorithm
#### G22: Make Logical Dependencies Physical
#### G23: Prefer Polymorphism to If/Else or Switch/Case
#### G24: Follow Standard Conventions
#### G25: Replace Magic Numbers with Named Constants
#### G26: Be Precise
#### G27: Structure over Convention
#### G28: Encapsulate Conditionals
#### G29: Avoid Negative Conditionals
#### G30: Functions Should Do One Thing
#### G31: Hidden Temporal Couplings
#### G32: Don’t Be Arbitrary
#### G33: Encapsulate Boundary Conditions
#### G34: Functions Should Descend Only

### One Level of Abstraction
#### G35: Keep Configurable Data at High Levels
#### G36: Avoid Transitive Navigation

## Java
#### J1: Avoid Long Import Lists by Using Wildcards
#### J2: Don’t Inherit Constants
#### J3: Constants versus Enums

### Names
#### N1: Choose Descriptive Names
#### N2: Choose Names at the Appropriate Level of Abstraction
#### N3: Use Standard Nomenclature Where Possible
#### N4: Unambiguous Names
#### N5: Use Long Names for Long Scopes
#### N6: Avoid Encodings
#### N7: Names Should Describe Side-Effects

### Tests
#### T1: Insufficient Tests
#### T2: Use a Coverage Tool!
#### T3: Don’t Skip Trivial Tests
#### T4: An Ignored Test Is a Question about an Ambiguity
#### T5: Test Boundary Conditions
#### T6: Exhaustively Test Near Bugs
#### T7: Patterns of Failure Are Revealing
#### T8: Test Coverage Patterns Can Be Revealing
#### T9: Tests Should Be Fast

### Conclusion
### Bibliography

<!-- ////////////////////////////////////////////////////////  -->
<!-- ////////////////////////////////////////////////////////  -->
<!-- ////////////////////////////////////////////////////////  -->
