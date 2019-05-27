---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bd9d53bd362eced1ab6918e8d6fa92f47471daba
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468020"
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