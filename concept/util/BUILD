#
# GRAKN.AI - THE KNOWLEDGE GRAPH
# Copyright (C) 2019 Grakn Labs Ltd
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU Affero General Public License as
# published by the Free Software Foundation, either version 3 of the
# License, or (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU Affero General Public License for more details.
#
# You should have received a copy of the GNU Affero General Public License
# along with this program.  If not, see <https://www.gnu.org/licenses/>.
#
#
package(default_visibility = ["//visibility:public"])

load("@graknlabs_build_tools//checkstyle:rules.bzl", "checkstyle_test")

java_library(
    name = "util",
    srcs = ["ConceptUtils.java"],
    tags = ["maven_coordinates=io.grakn.core:grakn-concept-util:{pom_version}"],
    deps = [
        "//kb/concept/api",
        "//kb/concept/structure",
        "//concept/impl",
        "//core",

        # External dependencies from Maven
        "//dependencies/maven/artifacts/com/google/code/findbugs:jsr305",
        "//dependencies/maven/artifacts/com/google/guava",
        "//dependencies/maven/artifacts/org/apache/tinkerpop:gremlin-core",
    ],
)

checkstyle_test(
    name = "checkstyle",
    targets = [
        ":util",
    ],
)
