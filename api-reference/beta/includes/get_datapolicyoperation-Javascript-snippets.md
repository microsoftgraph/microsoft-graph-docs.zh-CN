---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c282631f50e5ac46a84298651a0f5ba6b64c9e0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/dataPolicyOperations/{id}')
    .version('beta')
    .get();

```