---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f51a5fa2ba4570220696736ebbe80af0e7e7086c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705172"
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