---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bd025bbe7c1f1b9e74ef89f541e89e95680941e
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
  userInputType: "textBox"
};

let res = await client.api('/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}')
    .version('beta')
    .update(identityUserFlowAttributeAssignment);

```