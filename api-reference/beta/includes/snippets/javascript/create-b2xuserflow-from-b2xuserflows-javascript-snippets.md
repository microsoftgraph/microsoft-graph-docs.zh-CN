---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 559fcf19b4e6f91c73d6fded85301ec43e6c6325
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: "Partner",
    userFlowType: "signUpOrSignIn",
    userFlowTypeVersion: 1
};

let res = await client.api('/identity/b2xUserFlows')
    .version('beta')
    .post(b2xIdentityUserFlow);

```