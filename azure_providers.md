# Main Azure Resource Providers

This page contains a code snippet to register the main Azure providers on a new dev/test subscription. For production susbcription, adopt a less privilege design by registering only the mandatory resource providers.

```
for service in \
Microsoft.AAD \
Microsoft.Advisor \
Microsoft.AlertsManagement \
Microsoft.ApiManagement \
Microsoft.App \
Microsoft.AppConfiguration \
Microsoft.AppPlatform \
Microsoft.Automation \
Microsoft.AzureActiveDirectory \
Microsoft.BotService \
Microsoft.Cache \
Microsoft.Cdn \
Microsoft.CertificateRegistration \
Microsoft.Communication \
Microsoft.Compute \
Microsoft.ContainerInstance \
Microsoft.ContainerRegistry \
Microsoft.ContainerService \
Microsoft.CognitiveServices \
Microsoft.CostManagementExports \
Microsoft.CustomProviders \
Microsoft.DBforMySQL \
Microsoft.DBforPostgreSQL \
Microsoft.DevCenter \
Microsoft.DevOpsInfrastructure \
Microsoft.DomainRegistration \
Microsoft.DocumentDB \
Microsoft.EventGrid \
Microsoft.EventHub \
Microsoft.KeyVault \
Microsoft.Logic \
Microsoft.MachineLearningServices \
Microsoft.Maps \
Microsoft.ManagedIdentity \
Microsoft.Management \
Microsoft.Network \
Microsoft.NotificationHubs \
Microsoft.OperationalInsights \
Microsoft.OperationsManagement \
Microsoft.PowerPlatform \
Microsoft.Relay \
Microsoft.Scheduler \
Microsoft.Search \
Microsoft.Security \
Microsoft.ServiceBus \
Microsoft.Sql \
Microsoft.Storage \
Microsoft.VirtualMachineImages \
microsoft.visualstudio \
Microsoft.Web
do
    az provider register --namespace $service
done
```
