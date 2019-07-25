---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bd9d53bd362eced1ab6918e8d6fa92f47471daba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722123"
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
  ],
};

let res = await client.api('/schemaExtensions/{id}')
    .update({schemaExtension : schemaExtension});

```