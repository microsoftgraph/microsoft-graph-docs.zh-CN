---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4518ad5686acd9ccd9c274a1003a53650471adc4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: "displayName-value",
  templateId: "templateId-value",
  values: [
    {
      name: "CustomBlockedWordsList",
      value: ""
    },
    {
      name: "EnableMSStandardBlockedWords",
      value: "False"
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
      value: "False"
    },
    {
      name: "AllowGuestsToAccessGroups",
      value: "True"
    },
    {
      name: "GuestUsageGuidelinesUrl",
      value: ""
    },
    {
      name: "GroupCreationAllowedGroupId",
      value: "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      name: "AllowToAddGuests",
      value: "True"
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
      value: "True"
    }
  ]
};

let res = await client.api('/groupSettings/{id}')
    .update(groupSetting);

```