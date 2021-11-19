---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ced38cbe175e33f327954bc25aa11e30f4321901
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100306"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "adDomainPassword": "AdDomainPassword value",
}
options := &msgraphsdk.UpdateAdDomainPasswordRequestBuilderPatchOptions{
    Body: requestBody,
}
cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).UpdateAdDomainPassword().Patch(options)


```