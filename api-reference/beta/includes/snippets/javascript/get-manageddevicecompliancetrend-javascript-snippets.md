---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c6072a655765a5bd14f350ae6afa489bf8f23e0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441613"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managedDeviceComplianceTrend = await client.api('/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}')
    .version('beta')
    .get();

```