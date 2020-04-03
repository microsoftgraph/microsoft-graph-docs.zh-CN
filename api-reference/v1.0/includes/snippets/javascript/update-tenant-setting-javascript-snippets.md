---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdc86ff1b9abaf04024c889184ec1520556b5a4b
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: "Group.Unified",
  templateId: "62375ab9-6b52-47ed-826b-58e47e0e304b",
  values: [
    {
      name: "EnableMIPLabels",
      value: "false"
    },
    {
      name: "CustomBlockedWordsList",
      value: ""
    },
    {
      name: "EnableMSStandardBlockedWords",
      value: "false"
    },
    {
      name: "ClassificationDescriptions",
      value: ""
    },
    {
      name: "DefaultClassification",
      value: ""
    },
    {
      name: "PrefixSuffixNamingRequirement",
      value: ""
    },
    {
      name: "AllowGuestsToBeGroupOwner",
      value: "false"
    },
    {
      name: "AllowGuestsToAccessGroups",
      value: "true"
    },
    {
      name: "GuestUsageGuidelinesUrl",
      value: ""
    },
    {
      name: "GroupCreationAllowedGroupId",
      value: ""
    },
    {
      name: "AllowToAddGuests",
      value: "true"
    },
    {
      name: "UsageGuidelinesUrl",
      value: ""
    },
    {
      name: "ClassificationList",
      value: ""
    },
    {
      name: "EnableGroupCreation",
      value: "true"
    }
  ]
};

let res = await client.api('/groupSettings/{id}')
    .update(groupSetting);

```