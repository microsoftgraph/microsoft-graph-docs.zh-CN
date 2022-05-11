---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10dd6abf9c80c6f804c824dff45c4ae2fc03e0b6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327069"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupSetting()
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
result, err := graphClient.GroupSettings().Post(requestBody)


```