---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebbbb71f25de1095ec6cf60654dfa0eee29baf03
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedApproval = {
  userId: 'userId-value',
  roleId: 'roleId-value',
  approvalType: 'approvalType-value',
  approvalState: 'approvalState-value',
  approvalDuration: 'datetime-value'
};

await client.api('/privilegedApproval')
    .version('beta')
    .post(privilegedApproval);

```