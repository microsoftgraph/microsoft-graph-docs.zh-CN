---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6ea2589847869b8034246e47e8eedb8f2beb2d1e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439902"
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
    .post({privilegedApproval : privilegedApproval});

```