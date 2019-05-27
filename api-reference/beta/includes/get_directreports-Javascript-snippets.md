---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a6aef214b36397ab4371db0175aa2398d1de759d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/directReports')
    .version('beta')
    .get();

```