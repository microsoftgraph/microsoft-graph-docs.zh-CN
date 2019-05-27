---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f4a94b12db2601efbf5ff3cfec81b485bb5f4900
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/resetUnseenCount')
    .version('beta')
    .post();

```