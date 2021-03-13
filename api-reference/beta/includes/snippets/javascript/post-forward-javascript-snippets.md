---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d947741a5f218be3d9bafb82dae2c8b4c95a2c9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  comment: 'comment-value',
  toRecipients: [
    {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    }
  ]
};

await client.api('/groups/{id}/threads/{id}/posts/{id}/forward')
    .version('beta')
    .post(forward);

```