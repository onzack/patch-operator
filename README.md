# patch-operator
A simple patch operator for Kubernetes to update the image value in resources to match the current year and month (YYYY-MM e.g. 2021-01).  
The patch-operator uses a simple bash script with `kubectl patch` commands to update the image of a specific resource.  
The patch-operator is started as a Kubernetes cronJob with a default hourly schedule.

This project is in alpha stage.

# Installation
Install the patch-operator Helm Chart:  
1. Clone this repository:  
`git clone https://github.com/onzack/patch-operator.git`
2. Adjust values.yaml file:  
`cp ./patch-operator/Helm/patch-operator/values.yaml ./custom-values.yaml`  
`vim ./custom-values.yaml`
3. Install Helm Chart:  
`helm install -f custom-values.yaml -n <target app namespace> patch-operator ./patch-operator/Helm/patch-operator`

# Licence
Copyright 2021 ONZACK  

Licensed under the Apache License, Version 2.0 (the "License");  
you may not use this file except in compliance with the License.  
You may obtain a copy of the License at  

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software  
distributed under the License is distributed on an "AS IS" BASIS,  
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
See the License for the specific language governing permissions and  
limitations under the License.  
