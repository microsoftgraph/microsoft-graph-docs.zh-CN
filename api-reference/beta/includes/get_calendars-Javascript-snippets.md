---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a29dc08dfc7b80e551a3130a591e069417a1713
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendars')
    .version('beta')
    .get();

```