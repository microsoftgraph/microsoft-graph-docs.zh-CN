---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b171198595dd9eb271f90167b2ed6f660c9a598b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/2txjA-BMZEq-bKi6Wfj5aGQAB1OJ/buckets')
    .version('beta')
    .get();

```