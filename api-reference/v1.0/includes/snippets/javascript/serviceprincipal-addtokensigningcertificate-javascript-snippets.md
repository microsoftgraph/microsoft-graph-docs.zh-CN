---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04c43b75295094bcd09f33ed844b20273f4fa0cb
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335460"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addTokenSigningCertificate = {
    displayName: 'CN=customDisplayName',
    endDateTime: '2024-01-25T00:00:00Z'
};

await client.api('/servicePrincipals/004375c5-6e2e-4dec-95e3-626838cb9f80/addTokenSigningCertificate')
    .post(addTokenSigningCertificate);

```