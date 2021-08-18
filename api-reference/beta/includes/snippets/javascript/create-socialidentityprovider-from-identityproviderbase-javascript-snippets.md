---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fbeb75485cbb03f616290493f9c3721848624cb93cee00d9d0ca62d2fa132d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': 'microsoft.graph.socialIdentityProvider',
  displayName: 'Login with Amazon',
  identityProviderType: 'Amazon',
  clientId: '56433757-cadd-4135-8431-2c9e3fd68ae8',
  clientSecret: '000000000000'
};

await client.api('/identity/identityProviders')
    .version('beta')
    .post(identityProviderBase);

```