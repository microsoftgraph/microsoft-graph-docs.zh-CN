---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3f79c9143fa3b65ba204c5bb5b7b7d8ff1806ff
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': '#microsoft.graph.socialIdentityProvider',
  clientSecret: '1111111111111'
};

await client.api('/identity/identityProviders/Amazon-OAUTH')
    .version('beta')
    .update(identityProviderBase);

```