---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94cca184727e0d00141d1d7f142464a98e70b5f939f8ebae952a24bd7117ca20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentMultiple = await client.api('/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096')
    .version('beta')
    .expand('roleDefinition')
    .get();

```