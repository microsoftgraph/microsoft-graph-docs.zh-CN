---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 671c15778d16f34aee60dfe21136508ee2dc9593
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveRoleAssignments = await client.api('/roleManagement/directory/transitiveRoleAssignments')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('principalId eq \'2c7936bc-3517-40f3-8eda-4806637b6516\'')
    .get();

```