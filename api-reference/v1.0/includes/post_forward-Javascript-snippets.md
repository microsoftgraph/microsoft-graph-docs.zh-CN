---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eeb8cd0e3a19e639811352a45f9b44e4a6b59bb9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  comment: "comment-value",
  toRecipients: [
    {
      emailAddress: {
        name: "name-value",
        address: "address-value"
      }
    }
  ]
};

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/forward')
    .post(forward);

```