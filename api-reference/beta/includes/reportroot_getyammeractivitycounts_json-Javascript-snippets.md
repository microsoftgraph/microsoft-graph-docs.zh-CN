---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b24b5a391f601c9f73042f608b9ef7992b7d367
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478928"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerActivityCounts(period='D7')')
    .version('beta')
    .get();

```