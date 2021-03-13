---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60068831b4f3edda32a6d78999a9069e94ba2f1e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xIdentityUserFlow = await client.api('/identity/b2xUserFlows/{id}')
    .version('beta')
    .get();

```