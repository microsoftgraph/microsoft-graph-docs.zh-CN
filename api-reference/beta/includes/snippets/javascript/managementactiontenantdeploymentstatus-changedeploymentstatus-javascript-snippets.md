---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 532c1d362765b75e798833bbdc2a79d2007428ced04a7e5cd71976f745e5045d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219443"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const managementActionDeploymentStatus = {
  tenantGroupId: 'String',
  tenantId: 'String',
  managementActionId: 'String',
  managementTemplateId: 'String',
  status: 'String'
};

await client.api('/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus')
    .version('beta')
    .post(managementActionDeploymentStatus);

```