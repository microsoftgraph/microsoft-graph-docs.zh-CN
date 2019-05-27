---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f8f5f73a419abfaee949863598af6d0ee448e417
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const list = {
  name: "Books",
  columns: [
    {
      name: "Author",
      text: { }
    },
    {
      name: "PageCount",
      number: { }
    }
  ],
  list: {
    template: "genericList"
  }
};

let res = await client.api('/sites/{site-id}/lists')
    .version('beta')
    .post({list : list});

```