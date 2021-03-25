---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1780a5a4dd8fcde660c08c1accb705edb4e27446
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202511"
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

await client.api('/servicePrincipals/7c8d4399-b4bf-413a-8b6a-c577790cae7d/addTokenSigningCertificate')
    .version('beta')
    .post(selfSignedCertificate);

```