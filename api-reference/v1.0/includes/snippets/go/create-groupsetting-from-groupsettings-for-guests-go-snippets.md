---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca274379e96b27490bd18b1fbd86beb1bbbb1dd2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104200"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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