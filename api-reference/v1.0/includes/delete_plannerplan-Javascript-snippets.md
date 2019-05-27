---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b3039f508192013f4b74e99c20b5b8a06a1bef1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{id}')
    .delete();

```