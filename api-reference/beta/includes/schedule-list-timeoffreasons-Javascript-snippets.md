---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7e2766cca2c2cff2b9ff2007d5557d525bb3fc31
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .version('beta')
    .get();

```