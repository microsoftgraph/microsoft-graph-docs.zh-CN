---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 084e21734136459fa7fd9eaa0d018c61f41f933c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUsers = await client.api('/tenantRelationships/managedTenants/riskyUsers')
    .version('beta')
    .get();

```