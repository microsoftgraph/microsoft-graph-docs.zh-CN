---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 425d5dcccd84b9b33597c9ed6c80faab655f86c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/servicePrincipals/{id}/memberOf')
    .version('beta')
    .get();

```