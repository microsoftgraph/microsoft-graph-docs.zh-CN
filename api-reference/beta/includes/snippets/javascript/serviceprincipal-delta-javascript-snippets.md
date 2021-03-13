---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bff8c6ae2caba4821b6ef64a547e379a2347a1eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/servicePrincipals/delta')
    .version('beta')
    .get();

```