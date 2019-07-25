---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5389e376782c1934937e3e383772dafaee48c33d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711939"
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