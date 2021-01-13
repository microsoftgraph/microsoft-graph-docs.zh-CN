---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22aaa036282d7ba4df3e689e756bbedf5f481bd2
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
  displayName: "New Test API",
  targetUrl: "https://otherapi.com/api/endpoint",
  authenticationConfiguration: {
    @odata.type: "microsoft.graph.basicAuthentication",
    username:"<NEW_USERNAME>", 
    password:"<NEW_PASSWORD>"
  }
};

let res = await client.api('/identity/apiConnectors/{identityApiConnectorId}')
    .version('beta')
    .update(identityApiConnector);

```