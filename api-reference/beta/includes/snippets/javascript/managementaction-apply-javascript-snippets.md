---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8f67d74e59a794b4a31978eff26d395b1e0ea51484df31c54a4b13e3621803a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const managementActionDeploymentStatus = {
  tenantId: 'String',
  tenantGroupId: 'String',
  managementTemplateId: 'String'
};

await client.api('/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply')
    .version('beta')
    .post(managementActionDeploymentStatus);

```