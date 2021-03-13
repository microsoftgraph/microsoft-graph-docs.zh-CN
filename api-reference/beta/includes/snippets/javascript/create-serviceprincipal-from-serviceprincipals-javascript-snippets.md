---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1c8874cdfaacbd5165f1629a3490d90fa3e0fd6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798389"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: '65415bb1-9267-4313-bbf5-ae259732ee12',
};

await client.api('/servicePrincipals')
    .version('beta')
    .post(servicePrincipal);

```