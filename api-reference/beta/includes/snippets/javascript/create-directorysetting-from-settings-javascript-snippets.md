---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa0365413bb2422897a4660af7e9941b304bf27a
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  displayName: 'Group.Unified',
  templateId: '62375ab9-6b52-47ed-826b-58e47e0e304b',
  values: [
    {
      name: 'GuestUsageGuidelinesUrl',
      value: 'https://privacy.contoso.com/privacystatement'
    },
    {
      name: 'EnableMSStandardBlockedWords',
      value: 'true'
    },
    {
      name: 'EnableMIPLabels',
      value: 'true'
    },
    {
      name: 'PrefixSuffixNamingRequirement',
      value: '[Contoso-][GroupName]'
    }
  ]
};

await client.api('/settings')
    .version('beta')
    .post(directorySetting);

```