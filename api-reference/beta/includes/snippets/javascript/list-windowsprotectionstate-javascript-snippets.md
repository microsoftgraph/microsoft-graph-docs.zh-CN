---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc129873b9469fc11d81ddc2db90c2c460256c510e61f4f45b2d3fd9300a2d54
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsProtectionStates = await client.api('/tenantRelationships/managedTenants/windowsProtectionStates')
    .version('beta')
    .get();

```