---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 214c0a91ee4ab17c0f480c2c40992e6b2602554e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: "none"
};

let res = await client.api('/app/calls/{id}/reject')
    .version('beta')
    .post(reject);

```