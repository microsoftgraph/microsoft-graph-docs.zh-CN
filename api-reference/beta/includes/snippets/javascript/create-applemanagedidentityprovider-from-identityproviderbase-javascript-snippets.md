---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69db9677ad62868f0b7fdc1af97a827be96ff6f7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664693"
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
    .version('beta')
    .post(identityProviderBase);

```