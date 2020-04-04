# patch-operator
A simple patch operator for Kubernetes to update the image value in resources.  
The patch-operator uses a simple bash script with `kubectl patch` commands to update the image of a specific resource.  
The patch-operator is started as a Kubernetes cronJob with a default hourly schedule.

# Licence
Copyright 2020 dmlabs  

Licensed under the Apache License, Version 2.0 (the "License");  
you may not use this file except in compliance with the License.  
You may obtain a copy of the License at  

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software  
distributed under the License is distributed on an "AS IS" BASIS,  
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
See the License for the specific language governing permissions and  
limitations under the License.  
