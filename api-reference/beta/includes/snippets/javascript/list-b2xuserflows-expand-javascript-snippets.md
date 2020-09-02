---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b40bffe8b4dc5b3a54f5fad050f5dff400817f14
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2xUserFlows')
    .version('beta')
    .expand('identityProviders')
    .get();

```