---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: febce59ab894503c42de1ea687ae6fdc8b16cc40
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlow = {
  id: 'Pol1',
  userFlowType: 'signUpOrSignIn',
  userFlowTypeVersion: 1
};

await client.api('/identity/userFlows')
    .version('beta')
    .post(identityUserFlow);

```