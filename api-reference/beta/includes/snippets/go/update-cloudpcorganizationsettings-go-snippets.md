---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 741c5214740010c62b14ade530b41ef01d6c20ac
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220283"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcOrganizationSettings()
userAccountType := "standardUser"
requestBody.SetUserAccountType(&userAccountType)
osVersion := "windows11"
requestBody.SetOsVersion(&osVersion)
windowsSettings := msgraphsdk.NewCloudPcWindowsSettings()
requestBody.SetWindowsSettings(windowsSettings)
language := "en-US"
windowsSettings.SetLanguage(&language)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
}
options := &msgraphsdk.OrganizationSettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.DeviceManagement().VirtualEndpoint().OrganizationSettings().Patch(options)


```