---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9fa7c27e7b2360818f576d9381ab8cf61d113bae
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignments/my')
    .version('beta')
    .get();

```