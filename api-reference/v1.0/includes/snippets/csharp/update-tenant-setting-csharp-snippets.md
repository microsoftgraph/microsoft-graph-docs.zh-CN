---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee88362c7abfcae73dcf9561c3b46b5393901eb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778405"
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
            Value = "false"
        },
        new SettingValue
        {
            Name = "CustomBlockedWordsList",
            Value = ""
        },
        new SettingValue
        {
            Name = "EnableMSStandardBlockedWords",
            Value = "false"
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
            Value = "false"
        },
        new SettingValue
        {
            Name = "AllowGuestsToAccessGroups",
            Value = "true"
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
            Value = "true"
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
            Value = "true"
        }
    }
};

await graphClient.GroupSettings["{groupSetting-id}"]
    .Request()
    .UpdateAsync(groupSetting);

```