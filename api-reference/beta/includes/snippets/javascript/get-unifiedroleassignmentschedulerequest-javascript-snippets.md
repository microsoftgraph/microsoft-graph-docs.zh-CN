---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5242e5c860b7358014160d65acfcf15ab127b080
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentScheduleRequest = await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/b5a22921-656a-4429-9c4e-59a5f576614d')
    .version('beta')
    .get();

```