---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d5030c7a6d35a720dd6f82590d707811d46a1d2
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/ownedObjects')
    .version('beta')
    .get();

```