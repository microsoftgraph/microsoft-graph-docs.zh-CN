---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c9f703c05ceea0f1b6b685dbe1710859823be8a8765816d56fe4c94e9a19896
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  reason: 'reason-value',
  duration: 'duration-value',
  ticketNumber: 'ticketNumber-value',
  ticketSystem: 'ticketSystem-value'
};

await client.api('/privilegedRoles/{id}/selfActivate')
    .version('beta')
    .post(privilegedRoleAssignment);

```