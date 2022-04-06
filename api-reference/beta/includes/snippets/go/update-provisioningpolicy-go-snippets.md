---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94c89b321adb616c6dc6f2ce4c7f18ed307d2b3b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758823"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcProvisioningPolicy()
displayName := "HR provisioning policy"
requestBody.SetDisplayName(&displayName)
description := "Provisioning policy for India HR employees"
requestBody.SetDescription(&description)
onPremisesConnectionId := "4e47d0f6-6f77-44f0-8893-c0fe1701ffff"
requestBody.SetOnPremisesConnectionId(&onPremisesConnectionId)
imageId := "Image ID value"
requestBody.SetImageId(&imageId)
imageDisplayName := "Image Display Name value"
requestBody.SetImageDisplayName(&imageDisplayName)
imageType := "custom"
requestBody.SetImageType(&imageType)
windowsSettings := msgraphsdk.NewCloudPcWindowsSettings()
requestBody.SetWindowsSettings(windowsSettings)
language := "en-US"
windowsSettings.SetLanguage(&language)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
}
options := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Patch(options)


```