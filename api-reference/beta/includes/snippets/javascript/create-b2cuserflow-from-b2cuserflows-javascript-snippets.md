---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d287fe3fddf0fa2b49a9da1e458ec6a319b029ea4702b904d5949fd0daef6532
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
    id: 'Customer',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 3
};

await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```