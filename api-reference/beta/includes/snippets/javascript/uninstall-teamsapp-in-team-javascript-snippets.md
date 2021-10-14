---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86935ceb72b53364e600cf1be710610c42e89bbf496770bd9a45cfcfdeeeefa0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=')
    .version('beta')
    .delete();

```