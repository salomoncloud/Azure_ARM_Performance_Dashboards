# Azure_ARM_Performance_Dashboards
These workbooks shows performance counter data using parameterized queries and a high-level performance overview with drill-down capabilities. All identifiers and environment-specific values have been sanitized.

Both JSON files define Azure Monitor workbooks—custom dashboards used to visualize performance data for virtual machines—but they focus on slightly different aspects:

ARM_VM_Perf_Counters_Dashboard.json can be used to display detailed performance counter data. It sets up parameters (like workspace, time range, and counter selection) and includes a series of KQL queries that pull metrics (CPU, memory, network statistics) from the Perf table in Azure Monitor. The workbook helps users quickly identify and analyze performance counters for their VMs.

ARM_VM_Performance_Dashboard.json can be used to view overall VM performance. While it similarly establishes parameters and queries, it leverages insights from performance metrics (often using the InsightsMetrics data source) and organizes the information into different views (such as tabs for “Top 100 Machines” and “Top 10 Machines”). This dashboard gives users a comprehensive overview of VM performance trends and aggregates key metrics.

In summary, these can be used in enterprise environments for deep-dive counter analysis and a high-level performance overview with additional drill-down options.
