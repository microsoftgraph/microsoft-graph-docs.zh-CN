---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cfbcd9a5c62630693ab287d690fcc6cf68696af
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const selfSignedCertificate = {
    displayName: 'CN=customDisplayName',
    endDateTime: '2024-01-25T00:00:00Z'
};

await client.api('/servicePrincipals/004375c5-6e2e-4dec-95e3-626838cb9f80/addTokenSigningCertificate')
    .version('beta')
    .post(selfSignedCertificate);

```