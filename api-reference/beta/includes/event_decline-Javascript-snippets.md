---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0582e0d132931805a3ce3a5e0e0c9e65267f1fe2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/decline')
    .version('beta')
    .post(decline);

```