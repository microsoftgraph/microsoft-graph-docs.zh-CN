---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe84d9c2ef8fa92d2bc2af38697ee6a9e2f17c4d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{plan-id}/details')
    .get();

```