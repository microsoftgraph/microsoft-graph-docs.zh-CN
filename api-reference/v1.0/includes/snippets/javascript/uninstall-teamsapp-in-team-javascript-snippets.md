---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb9cd6d0a02d4688a0098bbcb94fe8ab088084ce92f012614270edce3df6990c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=')
    .delete();

```