---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac01bfc6396581fdd55dc46419d99537e30a7b79
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewGroupSetting()
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
options := &msgraphsdk.GroupSettingsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.GroupSettings().Post(options)


```