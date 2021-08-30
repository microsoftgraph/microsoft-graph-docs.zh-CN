---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 464e8a1c92d50b398869b3f5f8bf9d2d315d82f7844fe25f698088aa553eda98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831194"
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