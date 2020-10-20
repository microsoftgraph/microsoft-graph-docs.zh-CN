---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5087a5d06c8c5c28dde639bc1bb48af555b128d9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .get();

```