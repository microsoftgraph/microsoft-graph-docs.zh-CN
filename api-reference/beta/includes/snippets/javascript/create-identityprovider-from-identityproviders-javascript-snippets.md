---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e66c791b7bd67447edcf59df5c5b8c2086b09efe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  '@odata.type': 'microsoft.graph.identityProvider',
  name: 'Login with Amazon',
  type: 'Amazon',
  clientId: '56433757-cadd-4135-8431-2c9e3fd68ae8',
  clientSecret: '000000000000'
};

await client.api('/identityProviders')
    .version('beta')
    .post(identityProvider);

```