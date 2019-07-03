---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5389e376782c1934937e3e383772dafaee48c33d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```