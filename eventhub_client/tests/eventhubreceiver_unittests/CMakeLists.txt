#Copyright (c) Microsoft. All rights reserved.
#Licensed under the MIT license. See LICENSE file in the project root for full license information.

#this is CMakeLists.txt for eventhubreceiver_ut
cmake_minimum_required(VERSION 2.8.11)

compileAsC11()

set(theseTestsName eventhubreceiver_ut)

set(${theseTestsName}_test_files
    eventhubreceiver_unittests.c
)

set(${theseTestsName}_c_files
    ../../src/eventhubreceiver.c
)

set(${theseTestsName}_h_files
)

build_c_test_artifacts(${theseTestsName} ON "UnitTests")
