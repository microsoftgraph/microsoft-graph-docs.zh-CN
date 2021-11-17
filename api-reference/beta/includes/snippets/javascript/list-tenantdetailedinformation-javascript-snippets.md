---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b3dcbba861c59be14cd0ded80b39ef42d63f272d1e1cdedb837372d742647d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161208"
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