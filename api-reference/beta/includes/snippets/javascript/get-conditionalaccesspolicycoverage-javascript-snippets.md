---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 079adb4c233f36e885b5429987e6b89deef51619
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicyCoverage = await client.api('/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}')
    .version('beta')
    .get();

```