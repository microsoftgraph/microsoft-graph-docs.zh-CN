---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fabe0d50c47e8477ee2943e467bed1fdee65bca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800027"
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