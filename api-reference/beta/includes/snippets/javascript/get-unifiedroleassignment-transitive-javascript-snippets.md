---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c05eddc7469cf98a7b5a0558ce3d8ac6633f12e9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveRoleAssignments = await client.api('/roleManagement/directory/transitiveRoleAssignments')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('principalId eq \'2c7936bc-3517-40f3-8eda-4806637b6516\' and roleDefinitionId eq \'fe930be7-5e62-47db-91af-98c3a49a38b1\'')
    .get();

```