---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36d76fbd85cf2b8078b546a368799bf34d92082d9bbabcc1bbc1c7a43d88eb1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333028"
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