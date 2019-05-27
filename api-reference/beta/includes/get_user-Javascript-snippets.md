---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b576a2f53f1dab69a4518c87a9e41cfcf52085a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me')
    .version('beta')
    .get();

```