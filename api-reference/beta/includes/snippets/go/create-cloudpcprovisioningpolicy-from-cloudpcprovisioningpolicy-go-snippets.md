---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e596d2d3abb0ffb2313c96fa3bf6df3156d79747
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091347"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcProvisioningPolicy()
displayName := "Display Name value"
requestBody.SetDisplayName(&displayName)
description := "Description value"
requestBody.SetDescription(&description)
onPremisesConnectionId := "6bf90392-5fea-459a-9e9d-a2484abbffff"
requestBody.SetOnPremisesConnectionId(&onPremisesConnectionId)
imageId := "Image ID value"
requestBody.SetImageId(&imageId)
imageDisplayName := "Image Display Name value"
requestBody.SetImageDisplayName(&imageDisplayName)
imageType := "gallery"
requestBody.SetImageType(&imageType)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
}
options := &msgraphsdk.ProvisioningPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPolicies().Post(options)


```