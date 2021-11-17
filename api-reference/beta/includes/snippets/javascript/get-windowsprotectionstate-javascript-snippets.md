---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6a0a10739f78a5db48c1cd469c15a584e39463f9bafb4625e02362054a1e297
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333114"
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