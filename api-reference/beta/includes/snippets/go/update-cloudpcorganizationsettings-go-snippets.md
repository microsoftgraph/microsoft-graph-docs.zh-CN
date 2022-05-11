---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 371590a2b7c7fdaf0289ae1de6da1978c60e8db0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327555"
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
graphClient.DeviceManagement().VirtualEndpoint().OrganizationSettings().Patch(requestBody)


```