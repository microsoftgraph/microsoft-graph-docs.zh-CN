---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf7fa5f09c7a6f5a4c67f6fb3ad250172d8a5f7f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: 'Group.Unified',
  templateId: '62375ab9-6b52-47ed-826b-58e47e0e304b',
  values: [
    {
      name: 'EnableMIPLabels',
      value: 'false'
    },
    {
      name: 'CustomBlockedWordsList',
      value: ''
    },
    {
      name: 'EnableMSStandardBlockedWords',
      value: 'false'
    },
    {
      name: 'ClassificationDescriptions',
      value: ''
    },
    {
      name: 'DefaultClassification',
      value: ''
    },
    {
      name: 'PrefixSuffixNamingRequirement',
      value: ''
    },
    {
      name: 'AllowGuestsToBeGroupOwner',
      value: 'false'
    },
    {
      name: 'AllowGuestsToAccessGroups',
      value: 'true'
    },
    {
      name: 'GuestUsageGuidelinesUrl',
      value: ''
    },
    {
      name: 'GroupCreationAllowedGroupId',
      value: ''
    },
    {
      name: 'AllowToAddGuests',
      value: 'true'
    },
    {
      name: 'UsageGuidelinesUrl',
      value: ''
    },
    {
      name: 'ClassificationList',
      value: ''
    },
    {
      name: 'EnableGroupCreation',
      value: 'true'
    }
  ]
};

await client.api('/groupSettings/{id}')
    .update(groupSetting);

```