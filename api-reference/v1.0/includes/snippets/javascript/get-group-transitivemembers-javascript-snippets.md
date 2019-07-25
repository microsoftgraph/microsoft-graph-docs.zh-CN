---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8b2c75d9d5ee6275448a69892d3ea42fee16f4ef
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMembers')
    .get();

```