---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69481b1c9f0efc0fc062b5631c31c56e736cc73f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393989"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcOrganizationSettings()
userAccountType := "standardUser"
requestBody.SetUserAccountType(&userAccountType)
osVersion := "windows11"
requestBody.SetOsVersion(&osVersion)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
}
options := &msgraphsdk.OrganizationSettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().OrganizationSettings().Patch(options)


```