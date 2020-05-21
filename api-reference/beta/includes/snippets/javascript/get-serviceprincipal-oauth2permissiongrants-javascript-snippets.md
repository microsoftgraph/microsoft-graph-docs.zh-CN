---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e39afbb5c839940455d9a4838048c57385600974
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/oauth2PermissionGrants')
    .version('beta')
    .get();

```