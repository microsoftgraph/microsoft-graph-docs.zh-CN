---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16fe44ea8727ce9ea7b7e157bc70e37353e31f96680494e91b192223256c81a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
  userInputType: 'textBox'
};

await client.api('/identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/{id}')
    .update(identityUserFlowAttributeAssignment);

```