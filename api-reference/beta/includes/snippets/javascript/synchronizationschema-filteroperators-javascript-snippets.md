---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 132fa28bb9f66422afc0423070eb5ee0f24147ad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterOperators = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators')
    .version('beta')
    .get();

```