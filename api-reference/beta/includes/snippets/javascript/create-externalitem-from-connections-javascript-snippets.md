---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe855a236146234237bc86afbf514be1dda7be12
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573176"
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

await client.api('/external/connections/contosohr/items/TSP228082938')
    .version('beta')
    .put(externalItem);

```