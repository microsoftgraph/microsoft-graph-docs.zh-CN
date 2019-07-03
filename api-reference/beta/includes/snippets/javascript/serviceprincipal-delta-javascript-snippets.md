---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7db48d9ce03407aa90d82f0256322371c2e7c019
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/delta')
    .version('beta')
    .get();

```