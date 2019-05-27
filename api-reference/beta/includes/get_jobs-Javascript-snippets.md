---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d00d7b88b968bd642d9b1a48bc5d164c550f405f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/')
    .version('beta')
    .get();

```