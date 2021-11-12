---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5978dba585a75ac5e6ef99bce902331835ea2b134e78418af4b72741157b7ef3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantTag = {
  displayName: 'Onboarding',
  description: 'Tenants that we are currently onboarding'
};

await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}')
    .version('beta')
    .update(tenantTag);

```