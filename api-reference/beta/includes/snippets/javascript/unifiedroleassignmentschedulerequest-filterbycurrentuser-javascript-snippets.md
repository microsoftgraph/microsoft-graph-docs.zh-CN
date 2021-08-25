---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ef1a3b79c778881e75b544cee4f40d44ca25fde
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/RoleAssignmentScheduleRequests/filterByCurrentUser(on='principal')')
    .version('beta')
    .get();

```