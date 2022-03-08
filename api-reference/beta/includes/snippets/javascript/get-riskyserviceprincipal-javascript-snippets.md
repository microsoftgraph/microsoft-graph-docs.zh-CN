---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 402817e2e97b25c8db595c157725d0ad6e674464
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyServicePrincipal = await client.api('/identityProtection/riskyServicePrincipals/9089a539-a539-9089-39a5-899039a58990')
    .version('beta')
    .get();

```