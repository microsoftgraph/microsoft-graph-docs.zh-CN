---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb691d21cda3e13267e8eba847cac8256fd44892ab9f1c8f31850cd6cae10875
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106484"
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