---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b67e3e2ddf2c82d264b8c69b6bdf1f3142b3c0a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
  properties: [
    {
      name: 'new-name-value',
      type: 'new-type-value'
    },
    {
      name: 'additional-name-value',
      type: 'additional-type-value'
    }
  ]
};

await client.api('/schemaExtensions/{id}')
    .version('beta')
    .update(schemaExtension);

```