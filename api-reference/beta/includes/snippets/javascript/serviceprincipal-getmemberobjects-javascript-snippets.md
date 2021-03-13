---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d491bd136ba96e90191540da61aa07bb130e95a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/servicePrincipals/{id}/getMemberObjects')
    .version('beta')
    .post(string);

```