---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acd5c55e0ec4cf7961d9ba44ee63865b1d68f2e5
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser(on='target')')
    .version('beta')
    .get();

```