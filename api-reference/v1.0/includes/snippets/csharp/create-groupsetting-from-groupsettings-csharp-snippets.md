---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50a34f4c098fdb853451a7166bf560bb8deb20f5
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514681"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    DisplayName = "Group.Unified",
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