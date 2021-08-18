---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d77a7751b27c1c642c4004fee01f6a94856028f9
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userFlowIdentityProviders = {
  '@odata.id': 'https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test',
  '@odata.type': '#microsoft.graph.identityProvider'
};

await client.api('/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref')
    .version('beta')
    .update(userFlowIdentityProviders);

```