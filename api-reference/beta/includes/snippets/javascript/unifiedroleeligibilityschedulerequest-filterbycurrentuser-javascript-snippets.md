---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a95c129165406190279f1742b3b0b9f4b3cbfa5
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513733"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser(on='principal')')
    .version('beta')
    .get();

```