---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 057b8915709fc7ac8862c49dfc20aef354fd328f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managedDeviceCompliance = await client.api('/tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}')
    .version('beta')
    .get();

```