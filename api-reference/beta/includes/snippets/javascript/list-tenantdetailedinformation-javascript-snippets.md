---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 120bf9f2f128bf64e1499600aa5f89c8d54c3905
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantsDetailedInformation = await client.api('/tenantRelationships/managedTenants/tenantsDetailedInformation')
    .version('beta')
    .get();

```