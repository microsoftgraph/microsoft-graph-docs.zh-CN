---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bdd2895bfc375edd2f5f1cf4853bba6b569da14
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082647"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcUserSetting()
displayName := "Example"
requestBody.SetDisplayName(&displayName)
selfServiceEnabled := true
requestBody.SetSelfServiceEnabled(&selfServiceEnabled)
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