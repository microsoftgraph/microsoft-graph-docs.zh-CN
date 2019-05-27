---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f8624245f53816e7a2bfda41e4248ea4eb496a56
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .get();

```