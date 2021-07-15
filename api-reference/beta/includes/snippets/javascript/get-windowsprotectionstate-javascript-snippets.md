---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b34b90d62fcda4dc202db46242f5dcc672bcd67
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsProtectionState = await client.api('/tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}')
    .version('beta')
    .get();

```