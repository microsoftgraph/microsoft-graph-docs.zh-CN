---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a20b616773c6da57d164e5db8a06555ac39f124
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084701"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDirectorySetting()
displayName := "Group.Unified"
requestBody.SetDisplayName(&displayName)
templateId := "62375ab9-6b52-47ed-826b-58e47e0e304b"
requestBody.SetTemplateId(&templateId)
requestBody.SetValues( []SettingValue {
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "GuestUsageGuidelinesUrl",
        "value": "https://privacy.contoso.com/privacystatement",
    }
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "EnableMSStandardBlockedWords",
        "value": "true",
    }
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "EnableMIPLabels",
        "value": "true",
    }
    msgraphsdk.NewSettingValue(),
    SetAdditionalData(map[string]interface{}{
        "name": "PrefixSuffixNamingRequirement",
        "value": "[Contoso-][GroupName]",
    }
}
options := &msgraphsdk.SettingsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Settings().Post(options)


```