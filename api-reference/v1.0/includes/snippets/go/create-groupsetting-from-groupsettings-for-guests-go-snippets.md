---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10c1bb2e433fb28c83db23ffe6500238989fb6ff
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993117"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewGroupSetting()
displayName := "Group.Unified.Guest"
requestBody.SetDisplayName(&displayName)
templateId := "08d542b9-071f-4e16-94b0-74abb372e3d9"
requestBody.SetTemplateId(&templateId)
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "AllowToAddGuests",
        "value": "false",
    }
}
options := &msgraphsdk.SettingsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Settings().Post(options)


```