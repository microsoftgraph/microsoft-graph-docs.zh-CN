---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6371424c569b834c8a3116e592ba3fd730e7fc0ca4bb6c4d74daa389f419c871
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332854"
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