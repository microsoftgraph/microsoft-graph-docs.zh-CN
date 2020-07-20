---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 836f14f83bcb7ef5f1fc55d4143243f7548acfc7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationFlowsPolicy = {
  selfServiceSignUp: {
    isEnabled: true
  }
};

let res = await client.api('/policies/authenticationFlowsPolicy')
    .version('beta')
    .update(authenticationFlowsPolicy);

```