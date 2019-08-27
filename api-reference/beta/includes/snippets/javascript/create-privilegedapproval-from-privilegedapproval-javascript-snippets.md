---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3d949732fd774399ded97dc83a0bec5ac046d447
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636648"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedApproval = {
  userId: "userId-value",
  roleId: "roleId-value",
  approvalType: "approvalType-value",
  approvalState: "approvalState-value",
  approvalDuration: "datetime-value"
};

let res = await client.api('/privilegedApproval')
    .version('beta')
    .post(privilegedApproval);

```