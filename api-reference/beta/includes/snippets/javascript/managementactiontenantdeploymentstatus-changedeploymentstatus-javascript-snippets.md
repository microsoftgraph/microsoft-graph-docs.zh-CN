---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e4a60d0294a869360b726f162273be74faf47e5
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440921"
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