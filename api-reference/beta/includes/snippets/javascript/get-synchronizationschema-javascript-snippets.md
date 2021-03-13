---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a046178f29392e8ddb4fe4775f416afb99aa10b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790303"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationSchema = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .get();

```