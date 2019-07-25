---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b8edb3a31ae5e0132b784e96bfd169856d8bda7b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708936"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}/audioRoutingGroups')
    .version('beta')
    .get();

```