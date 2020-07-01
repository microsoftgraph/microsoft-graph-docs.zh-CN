---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55b93d4938121801bb2a2173288c2c95f9de1307
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45008839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
  properties: [
    {
      name:"new-name-value",
      type:"new-type-value"
    },
    {
      name:"additional-name-value",
      type:"additional-type-value"
    }
  ]
};

let res = await client.api('/schemaExtensions/{id}')
    .version('beta')
    .update(schemaExtension);

```