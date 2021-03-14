---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ea8c9e36b2deaf7f35e0f21751f3d93f14441ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const list = {
  displayName: 'Books',
  columns: [
    {
      name: 'Author',
      text: { }
    },
    {
      name: 'PageCount',
      number: { }
    }
  ],
  list: {
    template: 'genericList'
  }
};

await client.api('/sites/{site-id}/lists')
    .post(list);

```