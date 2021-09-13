---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6086e0c5d8a3a5616b74c8eebabcadcc21541c88b0af6c3cd3341d0e442c888
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334074"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}')
    .delete();

```