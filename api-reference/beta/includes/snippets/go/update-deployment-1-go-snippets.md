---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6010002b7fef8f72e88dc35f0b6362f3e44f44dd
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412487"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDeployment()
state := msgraphsdk.NewDeploymentState()
requestBody.SetState(state)
requestedValue := "paused"
state.SetRequestedValue(&requestedValue)
state.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
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