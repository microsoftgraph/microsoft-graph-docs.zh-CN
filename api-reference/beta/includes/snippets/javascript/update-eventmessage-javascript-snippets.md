---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 925f366a49eeb9dd629ad32c61c087db0f77a6ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: 'true',
};

await client.api('/me/messages/{id}')
    .version('beta')
    .update(message);

```