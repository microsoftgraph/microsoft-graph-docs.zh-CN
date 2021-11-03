---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc3a203c572bc030f06698f14df522673b30fd1c
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let response = await client.api('/tenantRelationships/managedTenants/riskyUsers/{riskyUserId}')
    .version('beta')
    .get();

```