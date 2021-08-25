---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ffee25286b1d375ea37c858f8b216db85dc350f
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516049"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentScheduleInstance = await client.api('/roleManagement/directory/roleAssignmentScheduleInstances/4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1')
    .version('beta')
    .get();

```