---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0910320ba742a25a8a92c40c402fdb39c2329e1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}')
    .version('beta')
    .delete();

```