---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 365e0231ba0270e67b55d85320ed249db396545f
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52870204"
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