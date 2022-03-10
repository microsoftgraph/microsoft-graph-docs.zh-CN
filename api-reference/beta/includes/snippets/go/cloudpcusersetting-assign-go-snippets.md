---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf34633bd17b3c3be8863ee0c6d102bc9579b809
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412169"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAssignmentsRequestBody()
requestBody.SetAssignments( []CloudPcUserSettingAssignment {
    msgraphsdk.NewCloudPcUserSettingAssignment(),
    SetAdditionalData(map[string]interface{}{
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
    }
}
options := &msgraphsdk.AssignRequestBuilderPostOptions{
    Body: requestBody,
}
cloudPcUserSettingId := "cloudPcUserSetting-id"
graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Assign(cloudPcUserSetting-id).Post(options)


```