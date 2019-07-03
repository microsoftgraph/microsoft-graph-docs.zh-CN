---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bc9a61013df39eb22e47560b52633cf26b47a91e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    DisplayName = "displayName-value",
    TemplateId = "templateId-value",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "CustomBlockedWordsList",
            Value = ""
        },
        new SettingValue
        {
            Name = "EnableMSStandardBlockedWords",
            Value = "False"
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
            Value = "False"
        },
        new SettingValue
        {
            Name = "AllowGuestsToAccessGroups",
            Value = "True"
        },
        new SettingValue
        {
            Name = "GuestUsageGuidelinesUrl",
            Value = ""
        },
        new SettingValue
        {
            Name = "GroupCreationAllowedGroupId",
            Value = "62e90394-69f5-4237-9190-012177145e10"
        },
        new SettingValue
        {
            Name = "AllowToAddGuests",
            Value = "True"
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
            Value = "True"
        }
    }
};

await graphClient.GroupSettings["{id}"]
    .Request()
    .UpdateAsync(groupSetting);

```