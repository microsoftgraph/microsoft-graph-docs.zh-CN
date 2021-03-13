---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a2ac436a82e03f2aba0534c53cfdfe1cb56f101
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/positions/{id}')
    .version('beta')
    .delete();

```