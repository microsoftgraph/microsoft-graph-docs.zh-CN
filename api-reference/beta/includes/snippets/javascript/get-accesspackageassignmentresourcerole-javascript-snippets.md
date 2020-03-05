---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 835e383b7899fd350ef61a64e9d02c507e41646e
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}')
    .version('beta')
    .get();

```