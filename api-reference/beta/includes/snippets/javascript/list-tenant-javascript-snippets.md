---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ca9a6e09df0acfe5fdb41b6a5354ea457d109e9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenants = await client.api('/tenantRelationships/managedTenants/tenants')
    .version('beta')
    .get();

```