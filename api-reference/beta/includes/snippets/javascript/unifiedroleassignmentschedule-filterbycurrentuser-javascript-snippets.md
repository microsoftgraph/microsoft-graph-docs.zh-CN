---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea28e13b4bb75f617080d6f6cb463996fe638559
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser(on='principal')')
    .version('beta')
    .get();

```