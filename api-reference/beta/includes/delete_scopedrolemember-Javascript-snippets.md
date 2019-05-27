---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3905a2858b9089f1e4369db8a7480d6a4905678a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .version('beta')
    .delete();

```