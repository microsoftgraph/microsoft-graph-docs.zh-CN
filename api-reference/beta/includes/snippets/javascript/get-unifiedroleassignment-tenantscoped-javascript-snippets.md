---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 390eff0b16ec9e79f14967e25e8976292832be91
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveRoleAssignments = await client.api('/roleManagement/directory/transitiveRoleAssignments')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('principalId eq \'2c7936bc-3517-40f3-8eda-4806637b6516\' and directoryScopeId eq \'/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2\'')
    .get();

```