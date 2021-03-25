---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 365e0231ba0270e67b55d85320ed249db396545f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209360"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principal-id}')
    .version('beta')
    .delete();

```