---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18473b930463df4cab7bc5765fdde86cd8ba9e35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
  displayName: 'New Test API',
  targetUrl: 'https://otherapi.com/api/endpoint',
  authenticationConfiguration: {
    '@odata.type': 'microsoft.graph.basicAuthentication',
    username: '<NEW_USERNAME>', 
    password: '<NEW_PASSWORD>'
  }
};

await client.api('/identity/apiConnectors/{identityApiConnectorId}')
    .version('beta')
    .update(identityApiConnector);

```