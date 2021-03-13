---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a05a5d7626e8db1810486f22300ee3c41b7341c9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationJob = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/')
    .version('beta')
    .get();

```