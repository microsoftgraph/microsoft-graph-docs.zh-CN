---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c70c579296e3be906de1bf9ff0d59c3bd1025c9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  '@odata.type': 'microsoft.graph.externalItem',
  acl: [
    {
      type: 'user',
      value: 'e811976d-83df-4cbd-8b9b-5215b18aa874',
      accessType: 'grant',
      identitySource: 'azureActiveDirectory'
    },
    {
      type: 'group',
      value: '14m1b9c38qe647f6a',
      accessType: 'deny',
      identitySource: 'external'
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
    .version('beta')
    .put(externalItem);

```