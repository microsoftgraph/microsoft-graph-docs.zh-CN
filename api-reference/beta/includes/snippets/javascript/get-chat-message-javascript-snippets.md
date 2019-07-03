---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3fac72fb98be0a82a0e2480ad3efd5d76ba79c5e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479880"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/chats/{id}')
    .version('beta')
    .get();

```