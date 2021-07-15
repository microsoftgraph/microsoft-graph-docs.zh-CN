---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f97014ad79d89f197cd91d95c175da4132a7f3d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442292"
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