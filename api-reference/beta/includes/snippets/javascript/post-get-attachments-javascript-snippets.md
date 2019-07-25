---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a7395d1031e047ce44ac69b45d9d588d0b3a233
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876003"
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