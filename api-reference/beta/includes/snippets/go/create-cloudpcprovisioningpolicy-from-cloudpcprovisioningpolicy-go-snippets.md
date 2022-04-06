---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 324dc1de7acde4548283ccd64b65a1f1c93c56f0
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759319"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcProvisioningPolicy()
description := "Description value"
requestBody.SetDescription(&description)
displayName := "Display Name value"
requestBody.SetDisplayName(&displayName)
domainJoinConfiguration := msgraphsdk.NewCloudPcDomainJoinConfiguration()
requestBody.SetDomainJoinConfiguration(domainJoinConfiguration)
onPremisesConnectionId := "16ee6c71-fc10-438b-88ac-daa1ccafffff"
domainJoinConfiguration.SetOnPremisesConnectionId(&onPremisesConnectionId)
domainJoinConfiguration.SetAdditionalData(map[string]interface{}{
    "domainJoinType": "hybridAzureADJoin",
}
id := "1d164206-bf41-4fd2-8424-a3192d39ffff"
requestBody.SetId(&id)
imageDisplayName := "Windows-10 19h1-evd"
requestBody.SetImageDisplayName(&imageDisplayName)
imageId := "MicrosoftWindowsDesktop_Windows-10_19h1-evd"
requestBody.SetImageId(&imageId)
imageType := "gallery"
requestBody.SetImageType(&imageType)
onPremisesConnectionId := "4e47d0f6-6f77-44f0-8893-c0fe1701ffff"
requestBody.SetOnPremisesConnectionId(&onPremisesConnectionId)
windowsSettings := msgraphsdk.NewCloudPcWindowsSettings()
requestBody.SetWindowsSettings(windowsSettings)
language := "en-US"
windowsSettings.SetLanguage(&language)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
}
options := &msgraphsdk.ProvisioningPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPolicies().Post(options)


```