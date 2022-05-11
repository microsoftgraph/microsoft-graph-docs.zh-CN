---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc08481d13b71bc6444b557f3d81c3c0819a5477
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327411"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDeployment()
content := msgraphsdk.NewDeployableContent()
requestBody.SetContent(content)
content.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2",
}
settings := msgraphsdk.NewDeploymentSettings()
requestBody.SetSettings(settings)
rollout := msgraphsdk.NewRolloutSettings()
settings.SetRollout(rollout)
devicesPerOffer := int32(100)
rollout.SetDevicesPerOffer(&devicesPerOffer)
monitoring := msgraphsdk.NewMonitoringSettings()
settings.SetMonitoring(monitoring)
monitoring.SetMonitoringRules( []MonitoringRule {
    msgraphsdk.NewMonitoringRule(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
        "signal": "rollback",
        "threshold": ,
        "action": "pauseDeployment",
    }
}
settings.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
}
result, err := graphClient.Admin().Windows().Updates().Deployments().Post(requestBody)


```