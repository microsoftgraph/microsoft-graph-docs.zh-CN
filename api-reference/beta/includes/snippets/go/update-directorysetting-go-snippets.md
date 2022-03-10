---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee8c70eac0a073d0e7a74795a6a2e636dad595c4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411672"
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
result, err := graphClient.SettingsById(&directorySettingId).Patch(options)


```