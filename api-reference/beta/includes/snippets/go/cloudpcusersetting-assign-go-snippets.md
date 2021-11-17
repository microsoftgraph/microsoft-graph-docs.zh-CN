---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4be01facf623f39e1819d03a13d911126c7c1a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018800"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
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
graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Assign().Post(options)


```