---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cac41c53e22baa6d25e778ca6b6488cf4862b0f4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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