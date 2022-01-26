---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c73dad715471836249c74a664b9c2974ada3ced
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225007"
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
graphClient.DeviceManagement().VirtualEndpoint().OrganizationSettings().Patch(options)


```