---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4767edfc46e2bb1ecda61970a5208fb7632ebacc
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528105"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDirectorySetting()
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "CustomBlockedWordsList",
        "value": "Contoso",
    }
}
options := &msgraphsdk.DirectorySettingRequestBuilderPatchOptions{
    Body: requestBody,
}
directorySettingId := "directorySetting-id"
graphClient.SettingsById(&directorySettingId).Patch(options)


```