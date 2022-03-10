---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e77de40c13a0696faccfde2885264bd29332c7a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411773"
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
graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).UpdateAdDomainPassword(cloudPcOnPremisesConnection-id).Patch(options)


```