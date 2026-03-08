1. Network Engineer submit a request with the Mikrotik configuration.
2. Need to create in host_vars a yaml file for each specific customer. Inside this yaml file,
we will insert each mikrotik device the customer has (organized by the site name: country-site-device).
Need to brainstorm how to retrieve the information from the sharefile and using an API with python to
create/add a hostvar.
3. Hostvars file will have the customer name, in the yaml file it will be separated by site name.
Each site will have each system name, admiral configs, 
4. group_var we put the mikrotik common configuration, such as hotspot, IP services, firewall, interfaces, radius, walled garden
configurations.
5. Run the 01_vars_creation playbook to 