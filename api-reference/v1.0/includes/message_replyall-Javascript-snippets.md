---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4fe3bde5536979c95d3d6f6a03761ed1d92df87a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
  comment: "comment-value"
};

let res = await client.api('/me/messages/{id}/replyAll')
    .post(replyAll);

```