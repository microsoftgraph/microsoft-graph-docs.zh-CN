---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e4583a3797ad7c2de43db203d51a9a2861fb0624514e6711d467208303e8716
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106859"
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