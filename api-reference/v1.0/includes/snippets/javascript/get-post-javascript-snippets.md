---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 18a9237877bb717816697f51dfaa80150079e489
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}')
    .get();

```