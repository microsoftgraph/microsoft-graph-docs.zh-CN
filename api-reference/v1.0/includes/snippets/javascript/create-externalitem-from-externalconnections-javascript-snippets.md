---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9397e458633994fd56b15810c99cd3aba11c70f
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579915"
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

await client.api('/connections/contosohr/items/TSP228082938')
    .put(externalItem);

```