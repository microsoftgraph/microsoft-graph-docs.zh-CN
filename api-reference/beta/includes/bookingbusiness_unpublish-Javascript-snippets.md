---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d6fab2e52b09d3042552d4d9b682874782a7110
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish')
    .version('beta')
    .post();

```