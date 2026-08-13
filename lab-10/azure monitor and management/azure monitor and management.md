# Azure Monitoring and Management

## Azure Monitor

### Explanation

Azure Monitor is a monitoring service that collects and analyzes telemetry from Azure resources, applications, and infrastructure.

It helps administrators monitor resource performance, availability, metrics, logs, and application health from a centralized platform.

### Steps to Use Azure Monitor

1. Sign in to the Azure Portal.
2. Search for **Monitor**.
3. Open **Azure Monitor**.
4. Select **Metrics** to view resource metrics.
5. Select the required **Subscription** and **Resource**.
6. Select the required metric.
7. Configure the required time range.
8. Review the monitoring data.
9. Use **Logs** when log-based analysis is required.

### Screenshot

![Azure Monitor](../screenshot/image10.png)

---

## Log Analytics

### Explanation

Log Analytics is a feature of Azure Monitor used to collect, query, and analyze log data stored in a Log Analytics workspace.

Administrators can use Kusto Query Language (KQL) to search logs and troubleshoot Azure resources and applications.

### Steps to Configure Log Analytics

1. Sign in to the Azure Portal.
2. Search for **Log Analytics workspaces**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Workspace name**.
7. Select the required **Region**.
8. Review the configuration.
9. Select **Review + create**.
10. Select **Create**.
11. Open the created workspace.
12. Select **Logs**.
13. Enter a KQL query.
14. Select **Run** to execute the query.

### Screenshot

![Log Analytics](../screenshot/image11.png)

---

## Application Insights

### Explanation

Application Insights is an application performance monitoring feature of Azure Monitor.

It helps monitor application availability, performance, failures, requests, dependencies, exceptions, and other application telemetry.

### Steps to Configure Application Insights

1. Sign in to the Azure Portal.
2. Search for **Application Insights**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Application Insights resource name**.
7. Select the required **Region**.
8. Select or create the required **Log Analytics workspace**.
9. Review the configuration.
10. Select **Review + create**.
11. Select **Create**.
12. Open the Application Insights resource.
13. Review application performance and telemetry data.

### Screenshot

![Application Insights](../screenshot/image12.png)

---

## Alerts

### Explanation

Azure Monitor alerts notify administrators when a monitored condition is met.

Alerts can be configured using metrics, log queries, activity log events, and other supported signals. An alert can trigger an action such as an email notification or an action group.

### Steps to Create an Alert

1. Sign in to the Azure Portal.
2. Search for **Alerts**.
3. Select **Create**.
4. Select **Alert rule**.
5. Select the required **Scope**.
6. Select the required **Condition**.
7. Configure the required signal and threshold.
8. Configure the **Actions** or Action Group.
9. Enter the required **Alert rule name**.
10. Review the configuration.
11. Select **Create alert rule**.

### Screenshot

![Azure Monitor Alert](../screenshot/image13.png)

---

## Azure Service Health

### Explanation

Azure Service Health provides information about Azure service issues that may affect your resources.

It includes information about service incidents, planned maintenance, health advisories, and other service-related events.

### Steps to Check Azure Service Health

1. Sign in to the Azure Portal.
2. Search for **Service Health**.
3. Open **Service Health**.
4. Select **Service issues** to view active incidents.
5. Select **Planned maintenance** to view upcoming maintenance.
6. Select **Health advisories** to view relevant advisories.
7. Review the affected services and regions.
8. Configure alerts if required.

### Screenshot

![Azure Service Health](../screenshot/image14.png)

---

## Azure Advisor

### Explanation

Azure Advisor analyzes Azure resources and provides recommendations to improve reliability, security, performance, operational excellence, and cost efficiency.

It helps administrators identify possible improvements in their Azure environment.

### Steps to Use Azure Advisor

1. Sign in to the Azure Portal.
2. Search for **Advisor**.
3. Open **Azure Advisor**.
4. Select the required **Subscription**.
5. Review the available recommendations.
6. Select a recommendation to view its details.
7. Review the potential benefits and required actions.
8. Implement the recommendation when appropriate.

### Screenshot

![Azure Advisor](../screenshot/image15.png)

---

## Activity Log

### Explanation

The Azure Activity Log records subscription-level events that occur in Azure.

It can be used to track operations such as resource creation, deletion, configuration changes, and administrative actions.

Activity Log data is useful for auditing, troubleshooting, and understanding changes made to Azure resources.

### Steps to View the Activity Log

1. Sign in to the Azure Portal.
2. Search for **Monitor**.
3. Open **Activity Log**.
4. Select the required **Subscription**.
5. Select the required **Resource** if necessary.
6. Configure the required time range.
7. Apply filters such as resource group, resource type, operation, or status.
8. Select an event to view its details.
9. Review the event information.

### Screenshot

![Azure Activity Log](../screenshot/image16.png)

---

