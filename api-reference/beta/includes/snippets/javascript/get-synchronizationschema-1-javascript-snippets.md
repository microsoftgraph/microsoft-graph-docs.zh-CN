---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a046178f29392e8ddb4fe4775f416afb99aa10b1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952943"
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