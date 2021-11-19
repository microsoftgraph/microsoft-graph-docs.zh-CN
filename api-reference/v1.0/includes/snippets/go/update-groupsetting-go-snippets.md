---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da87c697869a82122177411b5f9027969cc27486
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097833"
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
options := &msgraphsdk.GroupSettingRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
groupSettingId := "groupSetting-id"
graphClient.GroupsById(&groupId).SettingsById(&groupSettingId).Patch(options)


```