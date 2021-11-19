---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a3c935aa58b5b54c202150cfe0f8127f55afbe0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupSetting()
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "AllowToAddGuests",
        "value": "false",
    }
}
options := &msgraphsdk.GroupSettingRequestBuilderPatchOptions{
    Body: requestBody,
}
groupSettingId := "groupSetting-id"
graphClient.GroupSettingsById(&groupSettingId).Patch(options)


```