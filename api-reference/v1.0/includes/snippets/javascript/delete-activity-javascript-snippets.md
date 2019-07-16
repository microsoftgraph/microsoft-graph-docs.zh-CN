---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88109a17c9a88224081e8023cb2796e70b0c24d4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/activities/{activity-id}/')
    .delete();

```