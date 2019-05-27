---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5087a5d06c8c5c28dde639bc1bb48af555b128d9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .get();

```