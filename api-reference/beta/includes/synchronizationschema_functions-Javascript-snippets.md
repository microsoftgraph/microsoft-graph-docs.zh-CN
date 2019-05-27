---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 30941e358ffa975bcabbd6ac189f216d91215b5c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions')
    .version('beta')
    .get();

```