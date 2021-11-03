---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05edae9b6285945c926b39d1fb45d03a72757879
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: 'user',
      value: 'e811976d-83df-4cbd-8b9b-5215b18aa874',
      accessType: 'grant'
    },
    {
      type: 'externalGroup',
      value: '14m1b9c38qe647f6a',
      accessType: 'deny'
    }
  ],
  properties: {
    title: 'Error in the payment gateway',
    priority: 1,
    assignee: 'john@contoso.com'
  },
  content: {
    value: 'Error in payment gateway...',
    type: 'text'
  }
};

await client.api('/external/connections/contosohr/items/TSP228082938')
    .put(externalItem);

```