---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2519e3f7cbb91b3b1a5f21ae1fca0b03a2d7225
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211347"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedAdminCustomers = await client.api('/tenantRelationships/delegatedAdminCustomers')
    .version('beta')
    .get();

```