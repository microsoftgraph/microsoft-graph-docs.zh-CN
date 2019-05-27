---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c7e8c82f7bdee5c2a3b4e6686d1e1d9653ec9ba
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454816"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{plan-id}')
    .get();

```