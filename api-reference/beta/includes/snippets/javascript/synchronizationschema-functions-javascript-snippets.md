---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30941e358ffa975bcabbd6ac189f216d91215b5c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions')
    .version('beta')
    .get();

```