# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

configure_file (
  "orc/orc-config.hh.in"
  "${CMAKE_CURRENT_BINARY_DIR}/orc/orc-config.hh"
  )

install(FILES
  "${CMAKE_CURRENT_BINARY_DIR}/orc/orc-config.hh"
  "orc/ColumnPrinter.hh"
  "orc/Common.hh"
  "orc/Int128.hh"
  "orc/MemoryPool.hh"
  "orc/OrcFile.hh"
  "orc/Reader.hh"
  "orc/Type.hh"
  "orc/Vector.hh"
  "orc/Statistics.hh"
  DESTINATION "include/orc"
  )
