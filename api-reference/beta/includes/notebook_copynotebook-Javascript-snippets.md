---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa8c97bb3b2ec83f64192536f0f099b262c8e346
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443780"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  groupId: "groupId-value",
  renameAs: "renameAs-value"
};

let res = await client.api('/me/onenote/notebooks/{id}/copyNotebook')
    .version('beta')
    .post(onenoteOperation);

```