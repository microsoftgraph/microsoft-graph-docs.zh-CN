---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d6297908ee742c322b70c308ca25f376b736720
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098742"
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
signal := "rollback"
    SetSignal(&signal)
threshold := int32(5)
    SetThreshold(&threshold)
action := "pauseDeployment"
    SetAction(&action)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
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