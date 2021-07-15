---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 046e8d790e0034f0664caac2fa22f5cd09e1189c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantGroups = await client.api('/tenantRelationships/managedTenants/tenantGroups')
    .version('beta')
    .get();

```