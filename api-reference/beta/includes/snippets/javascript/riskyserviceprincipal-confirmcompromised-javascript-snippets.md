---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7af7cbc0a1100bd43cac8715275e38f00733b643
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmCompromised = {
  servicePrincipalIds: [
    '9089a539-a539-9089-39a5-899039a58990'
  ]
};

await client.api('/identityProtection/riskyServicePrincipals/confirmCompromised')
    .version('beta')
    .post(confirmCompromised);

```