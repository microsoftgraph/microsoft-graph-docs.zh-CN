---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 881eb3215da3503ded16cd0e12c004d6cc3c763d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```