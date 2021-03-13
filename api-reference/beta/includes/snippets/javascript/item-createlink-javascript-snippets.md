---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af0318ac4e8d4eb5090d872d458c53ee8e4d2783
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808851"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'view',
  password: 'ThisIsMyPrivatePassword',
  scope: 'anonymous'
};

await client.api('/me/drive/items/{itemId}/createLink')
    .version('beta')
    .post(permission);

```