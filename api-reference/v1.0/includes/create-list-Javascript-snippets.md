---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f51a5fa2ba4570220696736ebbe80af0e7e7086c
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const list = {
  displayName: "Books",
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
    .post({list : list});

```