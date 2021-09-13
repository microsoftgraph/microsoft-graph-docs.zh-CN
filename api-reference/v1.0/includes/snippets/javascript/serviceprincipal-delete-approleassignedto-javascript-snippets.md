---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c745ec67fcf6364a62aa8d3da5cd1a82ac070aca0768d41892586390edf83fa7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}')
    .delete();

```