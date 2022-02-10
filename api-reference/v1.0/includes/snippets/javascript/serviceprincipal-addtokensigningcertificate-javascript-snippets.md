---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3debb4b875a06bcaf58567b2f5c4d869aab42e24
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519220"
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
    .post(selfSignedCertificate);

```