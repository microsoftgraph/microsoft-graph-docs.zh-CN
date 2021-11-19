---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa85b90e658bce6c8b822cc405b118291a0824b4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102196"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcProvisioningPolicy()
displayName := "Display Name value"
requestBody.SetDisplayName(&displayName)
description := "Description value"
requestBody.SetDescription(&description)
onPremisesConnectionId := "4e47d0f6-6f77-44f0-8893-c0fe1701ffff"
requestBody.SetOnPremisesConnectionId(&onPremisesConnectionId)
imageId := "Image ID value"
requestBody.SetImageId(&imageId)
imageDisplayName := "Image Display Name value"
requestBody.SetImageDisplayName(&imageDisplayName)
imageType := "custom"
requestBody.SetImageType(&imageType)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
}
options := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Patch(options)


```