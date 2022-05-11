---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9023c745b6327271e4ca288c0c69b727e948204f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327063"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupSetting()
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "AllowToAddGuests",
        "value": "true",
    }
}
groupId := "group-id"
groupSettingId := "groupSetting-id"
graphClient.GroupsById(&groupId).SettingsById(&groupSettingId).Patch(requestBody)


```