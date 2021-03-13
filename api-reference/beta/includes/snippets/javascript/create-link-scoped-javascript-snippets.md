---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a92b0ff5aa28ae0669fcce4b706645a0f942c757
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'edit',
  scope: 'organization'
};

await client.api('/me/drive/items/{item-id}/createLink')
    .version('beta')
    .post(permission);

```