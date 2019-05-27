---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f03a2e09b5285b55ac3de6a3e3ce8cf7069bbd20
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details')
    .version('beta')
    .get();

```