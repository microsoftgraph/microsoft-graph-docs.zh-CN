---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39d61c7fcd4fc7926490e2819e36a59a291c0c06
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327017"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDirectorySetting()
templateId := "08d542b9-071f-4e16-94b0-74abb372e3d9"
requestBody.SetTemplateId(&templateId)
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "AllowToAddGuests",
        "value": "false",
    }
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Settings().Post(requestBody)


```