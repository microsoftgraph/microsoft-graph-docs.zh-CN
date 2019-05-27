---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 068f01e8378e4f63cf7325052cb271a2ce7d8c68
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{idOrUserPrincipalName}/drive')
    .version('beta')
    .get();

```