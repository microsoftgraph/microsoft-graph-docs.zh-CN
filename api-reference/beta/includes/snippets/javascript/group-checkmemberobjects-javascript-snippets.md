---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8da666736cb92d405cdbeed8b2f3dcdb8f3fba8e
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  ids: [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
};

let res = await client.api('/groups/{id}/checkMemberObjects')
    .version('beta')
    .post(String);

```