---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35ee0dcc0ea26e8f5bb096ea54d19e4d2dc40bdb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    TemplateId = "62375ab9-6b52-47ed-826b-58e47e0e304b",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "GuestUsageGuidelinesUrl",
            Value = "https://privacy.contoso.com/privacystatement"
        },
        new SettingValue
        {
            Name = "EnableMSStandardBlockedWords",
            Value = "true"
        },
        new SettingValue
        {
            Name = "EnableMIPLabels",
            Value = "true"
        },
        new SettingValue
        {
            Name = "PrefixSuffixNamingRequirement",
            Value = "[Contoso-][GroupName]"
        }
    }
};

await graphClient.GroupSettings
    .Request()
    .AddAsync(groupSetting);

```