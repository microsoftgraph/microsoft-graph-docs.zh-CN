---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88109a17c9a88224081e8023cb2796e70b0c24d4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/activities/{activity-id}/')
    .delete();

```