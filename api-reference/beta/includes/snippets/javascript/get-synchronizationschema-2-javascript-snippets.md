---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b097dd517f06c0c8adef98caeaf446f7bd4ced8f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956888"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationSchema = await client.api('/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .header('Authorization','Bearer {Token}')
    .get();

```