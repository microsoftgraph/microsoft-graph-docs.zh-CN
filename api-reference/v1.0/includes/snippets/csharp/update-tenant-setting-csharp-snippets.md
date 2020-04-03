---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0758fc7d939cd42cdd21d30441795116c5563df4
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947080"
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
            Name = "EnableMIPLabels",
            Value = false
        },
        new SettingValue
        {
            Name = "CustomBlockedWordsList",
            Value = ""
        },
        new SettingValue
        {
            Name = "EnableMSStandardBlockedWords",
            Value = false
        },
        new SettingValue
        {
            Name = "ClassificationDescriptions",
            Value = ""
        },
        new SettingValue
        {
            Name = "DefaultClassification",
            Value = ""
        },
        new SettingValue
        {
            Name = "PrefixSuffixNamingRequirement",
            Value = ""
        },
        new SettingValue
        {
            Name = "AllowGuestsToBeGroupOwner",
            Value = false
        },
        new SettingValue
        {
            Name = "AllowGuestsToAccessGroups",
            Value = true
        },
        new SettingValue
        {
            Name = "GuestUsageGuidelinesUrl",
            Value = ""
        },
        new SettingValue
        {
            Name = "GroupCreationAllowedGroupId",
            Value = ""
        },
        new SettingValue
        {
            Name = "AllowToAddGuests",
            Value = true
        },
        new SettingValue
        {
            Name = "UsageGuidelinesUrl",
            Value = ""
        },
        new SettingValue
        {
            Name = "ClassificationList",
            Value = ""
        },
        new SettingValue
        {
            Name = "EnableGroupCreation",
            Value = true
        }
    }
};

await graphClient.GroupSettings["{id}"]
    .Request()
    .UpdateAsync(groupSetting);

```