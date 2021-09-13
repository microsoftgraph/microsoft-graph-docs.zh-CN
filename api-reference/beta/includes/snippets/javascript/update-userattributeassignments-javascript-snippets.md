---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 721711402db0fd0775b8f9d38d95349a99bd251097921b462552d467003afcef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106144"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
  userInputType: 'textBox'
};

await client.api('/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}')
    .version('beta')
    .update(identityUserFlowAttributeAssignment);

```