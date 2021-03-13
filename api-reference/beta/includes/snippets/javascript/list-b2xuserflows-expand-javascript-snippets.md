---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c76fa4c439b3c5c453d4a38215e344b5521131c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .version('beta')
    .expand('identityProviders')
    .get();

```