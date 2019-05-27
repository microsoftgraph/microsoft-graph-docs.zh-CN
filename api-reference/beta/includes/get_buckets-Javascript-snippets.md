---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b171198595dd9eb271f90167b2ed6f660c9a598b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473615"
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