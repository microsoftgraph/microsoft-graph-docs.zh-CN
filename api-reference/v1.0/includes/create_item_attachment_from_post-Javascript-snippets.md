---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4ce45e7af5929485c96969529de4c24e31c2a94c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.itemAttachment",
  name: "name-value",
  item: { }
};

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/attachments')
    .post({attachment : attachment});

```