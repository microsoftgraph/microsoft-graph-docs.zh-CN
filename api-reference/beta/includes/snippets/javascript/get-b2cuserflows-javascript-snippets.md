---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a364eb3157f9d2312570bf2027d37c9e8e71e3e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792230"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cIdentityUserFlow = await client.api('/identity/b2cUserFlows/{id}')
    .version('beta')
    .get();

```