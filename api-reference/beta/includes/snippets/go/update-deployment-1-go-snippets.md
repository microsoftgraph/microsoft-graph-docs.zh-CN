---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9c9dc2218f3c06837e86c64f22854fb89422da5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095608"
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
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Patch(options)


```