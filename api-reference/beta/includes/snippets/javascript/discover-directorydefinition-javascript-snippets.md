---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6b11560f250a5ba16581d8172da7614ad008ee1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover')
    .version('beta')
    .post();

```