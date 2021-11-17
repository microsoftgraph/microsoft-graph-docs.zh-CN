---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8640fb204a4ec21f0d80c22321cb781e41ad4129
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': 'microsoft.graph.appleManagedIdentityProvider',
  displayName: 'Sign in with Apple',
  developerId: 'UBF8T346G9',
  serviceId: 'com.microsoft.rts.b2c.test.client',
  keyId: '99P6D879C4',
  certificateData: '******'
};

await client.api('/identity/identityProviders')
    .post(identityProviderBase);

```