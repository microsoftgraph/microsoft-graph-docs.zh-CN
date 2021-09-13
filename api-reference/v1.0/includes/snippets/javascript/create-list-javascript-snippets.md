---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60cdad754b7d40945527a009297090dcc6a40ba8683efe811cf9e95c6442d983
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409707"
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