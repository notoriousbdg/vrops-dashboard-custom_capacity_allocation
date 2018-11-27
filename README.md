
# Custom Capacity Allocation Overview Dashboard for vRealize Operations 6.7 and 7.0
---------

Use this [vRealize Operations](https://www.vmware.com/products/vrealize-operations.html) dashboard to implement custom allocation ratios.  This dashboard is a clone of the Capacity Allocation Overview dashboard customized to support a 2:1 vCPU and 1.1:1 vMem ratios.  This dashboard can be easily customized to suit any ratio by changing the ratio in the included super metrics.

## Dashboard
![Dashboard](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/master/Dashboard.png)

## Installation
1. Import the super metric at `Administration` / `Configuration` / `Super Metrics` / `Import Super Metric`  
![Import View](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/master/Import_Super_Metric.png)
2. Click `Browse...` then select the file named [SuperMetric - Custom Allocation Ratios.json](https://github.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/raw/master/SuperMetric%20-%20Custom%20Allocation%20Ratios.json)
3. Edit the Policy at `Administration` / `Policies` / `Policy Library`.  The policy should be `vSphere Solution's Default Policy (DATE)` unless a new policy was explicitly created.  
![Policy Library](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/master/Policy_Library.png)
4. Enable `Super Metric|vCPU Allocation % for 2 vCPU per Core (%)` and `Super Metric|vMem Allocatoin % for 1.1 Overcommitment per GB (%)` Super Metrics on Cluster Compute Resource objects only.
![Policy Metrics](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/master/Policy_Metrics.png)
5. Import the view at `Dashboards` / `Views` / `Import...`  
![Import View](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/master/Import_View.png)
6. Click `Browse...` then select the file named [Views - Custom Current Allocation Percentage for Clusters.zip](https://github.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/raw/master/Views%20-%20Custom%20Current%20Allocation%20Percentage%20for%20Clusters.zip)
7. Import the dashboard at `Dashboards` / `Actions` / `Manage Dashboards` / `Import Dashboards`  
![Import Dashboard](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/master/Import_Dashboard.png)
8. Click `Browse...` then select the file named [Dashboard - Custom Capacity Allocation Overview.zip](https://github.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/raw/master/Dashboard%20-%20Custom%20Capacity%20Allocation%20Overview.zip)
9. The dashboard should now be available in in the dashboard list  
![Dashboard List](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/master/Dashboard_List.png)

## Support

This dashboard requires vRealize Operation 6.7 (or newer) Advanced or Enterprise edition.

Please open an [issue](https://github.com/notoriousbdg/vrops-dashboard-custom_capacity_allocation/issues) for feedback.
