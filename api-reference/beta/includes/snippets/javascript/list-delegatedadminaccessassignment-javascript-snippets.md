---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f67ac483c279ff7ac097b26647d8a39fb6f1a794
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessAssignments = await client.api('/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments')
    .version('beta')
    .get();

```