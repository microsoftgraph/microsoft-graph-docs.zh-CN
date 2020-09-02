---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 093f0cf9a4d5945918ecc55fc120ca8b774cbf69
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2xUserFlows/{id}')
    .version('beta')
    .get();

```