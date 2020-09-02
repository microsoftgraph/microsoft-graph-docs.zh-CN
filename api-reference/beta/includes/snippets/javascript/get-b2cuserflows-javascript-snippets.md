---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f872d192021a2c344c5b753f234eb12858c16d
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/{id}')
    .version('beta')
    .get();

```