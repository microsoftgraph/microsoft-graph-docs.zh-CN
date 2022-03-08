---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e864fa4521c84fd120755dd2858a0a73e52998e6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335512"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcUserSetting()
displayName := "Example"
requestBody.SetDisplayName(&displayName)
selfServiceEnabled := true
requestBody.SetSelfServiceEnabled(&selfServiceEnabled)
restorePointSetting := msgraphsdk.NewCloudPcRestorePointSetting()
requestBody.SetRestorePointSetting(restorePointSetting)
frequencyInHours := "16"
restorePointSetting.SetFrequencyInHours(&frequencyInHours)
userRestoreEnabled := true
restorePointSetting.SetUserRestoreEnabled(&userRestoreEnabled)
localAdminEnabled := false
requestBody.SetLocalAdminEnabled(&localAdminEnabled)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
}
options := &msgraphsdk.CloudPcUserSettingRequestBuilderPatchOptions{
    Body: requestBody,
}
cloudPcUserSettingId := "cloudPcUserSetting-id"
graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Patch(options)


```