---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc57fe8f67108df786c09d1c1b83afc6fa2b47e4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: '65415bb1-9267-4313-bbf5-ae259732ee12'
};

await client.api('/servicePrincipals')
    .post(servicePrincipal);

```