---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e0bddc0e84f577bd701a0861fe1fa647487ef9a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade')
    .version('beta')
    .post();

```