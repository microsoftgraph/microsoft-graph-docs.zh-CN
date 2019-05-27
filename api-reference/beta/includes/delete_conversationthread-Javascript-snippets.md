---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 34873fe95c0657fb6f715084df0ce43cb77970a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .delete();

```