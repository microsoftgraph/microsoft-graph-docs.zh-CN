---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0976ea0975fecee37c47a17e14d7f77daf7fc6a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/'id'')
    .version('beta')
    .delete();

```