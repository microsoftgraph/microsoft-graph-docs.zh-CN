---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a7395d1031e047ce44ac69b45d9d588d0b3a233
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/attachments')
    .version('beta')
    .get();

```