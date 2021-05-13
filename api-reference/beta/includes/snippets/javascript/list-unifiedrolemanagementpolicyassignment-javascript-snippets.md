---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 483d545a0eeb725a76d129fef24f23453a0e80d0
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicyAssignments = await client.api('/policies/roleManagementPolicyAssignments')
    .version('beta')
    .get();

```