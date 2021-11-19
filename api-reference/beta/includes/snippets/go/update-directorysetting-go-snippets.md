---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c4c5515ac15638da6a7bc58f0aa6f428f83d66f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102792"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDirectorySetting()
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "name-value",
        "value": "value-value",
    }
}
options := &msgraphsdk.DirectorySettingRequestBuilderPatchOptions{
    Body: requestBody,
}
directorySettingId := "directorySetting-id"
graphClient.SettingsById(&directorySettingId).Patch(options)


```