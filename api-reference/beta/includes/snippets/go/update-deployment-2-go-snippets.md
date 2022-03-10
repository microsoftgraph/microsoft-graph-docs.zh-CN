---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b44242b82a2bfc32ff507fda581fe1332e532d10
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412488"
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
    SetAdditionalData(map[string]interface{}{
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
options := &msgraphsdk.DeploymentRequestBuilderPatchOptions{
    Body: requestBody,
}
deploymentId := "deployment-id"
result, err := graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Patch(options)


```