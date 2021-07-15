---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c4b06be3e2792541d0589167158d9a2bbbd7ba8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantDetailedInformation = await client.api('/tenantRelationships/managedTenants/tenantsDetailedInformation/{tenantDetailedInformationId}')
    .version('beta')
    .get();

```