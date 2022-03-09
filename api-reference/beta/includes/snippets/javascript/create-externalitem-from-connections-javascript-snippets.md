---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc0856ac06b4bbe3e74d6dea6a5eee68ec132d13ea6276f577ca80f2e609731
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161555"
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

await client.api('/external/connections/contosohr/items/TSP228082938')
    .version('beta')
    .put(externalItem);

```