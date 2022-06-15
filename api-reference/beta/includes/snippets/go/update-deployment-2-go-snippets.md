---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 478e1c7b0a933d31d457f78b370a3a816172f4d9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098683"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDeployment()
settings := msgraphsdk.NewDeploymentSettings()
requestBody.SetSettings(settings)
monitoring := msgraphsdk.NewMonitoringSettings()
settings.SetMonitoring(monitoring)
monitoring.SetMonitoringRules( []MonitoringRule {
    msgraphsdk.NewMonitoringRule(),
signal := "rollback"
    SetSignal(&signal)
threshold := int32(5)
    SetThreshold(&threshold)
action := "pauseDeployment"
    SetAction(&action)
}
settings.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
}
deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Patch(requestBody)


```