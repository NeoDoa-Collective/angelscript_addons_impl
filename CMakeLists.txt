cmake_minimum_required(VERSION 3.26.4)

project(angelscript_addons_impl)

add_library(
angelscript_addons_impl
"datetime.cpp"
"scriptany.cpp"
"scriptarray.cpp"
"scriptbuilder.cpp"
"scriptdictionary.cpp"
"scriptfile.cpp"
"scriptgrid.cpp"
"scripthandle.cpp"
"scripthelper.cpp"
"scriptmath.cpp"
"scriptstdstring.cpp")

find_package(Angelscript CONFIG REQUIRED)
target_link_libraries(angelscript_addons_impl PUBLIC Angelscript::angelscript)