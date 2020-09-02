---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 218bc2a8c64857247dd7af00e47f3a438cbad057
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329389"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2xUserFlows/{id}')
    .version('beta')
    .delete();

```