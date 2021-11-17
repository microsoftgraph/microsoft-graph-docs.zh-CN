---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f613aaa2a3374b4d9c69370b8fda467443c0becdf18fcd4d235ef16532dbe9aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277429"
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
    .version('beta')
    .post(list);

```