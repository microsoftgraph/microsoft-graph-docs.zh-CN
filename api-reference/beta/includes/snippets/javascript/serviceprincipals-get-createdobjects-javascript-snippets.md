---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0014628864279b1bfe16cf7dbc48010d77399685
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/createdObjects')
    .version('beta')
    .get();

```