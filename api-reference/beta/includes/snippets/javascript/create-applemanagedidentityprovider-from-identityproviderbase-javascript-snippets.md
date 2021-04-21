---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69db9677ad62868f0b7fdc1af97a827be96ff6f7
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921319"
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