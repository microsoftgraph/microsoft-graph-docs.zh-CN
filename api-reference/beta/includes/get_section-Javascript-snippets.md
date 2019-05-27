---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0fb2a4ea83b84b1f5331288f3b985d5bb6ffaccd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sections/{id}')
    .version('beta')
    .get();

```