---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7d2e7a47884f03cf739a6570da1e93781936624a
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34535978"
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
    .version('beta')
    .post({list : list});

```