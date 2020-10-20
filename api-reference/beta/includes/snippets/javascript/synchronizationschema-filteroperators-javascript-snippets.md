---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d23a859c11cb3168e2434230b0d3f4d0ad002575
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604391"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators')
    .version('beta')
    .get();

```