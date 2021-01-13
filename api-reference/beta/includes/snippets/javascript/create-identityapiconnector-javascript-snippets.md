---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 046ca8bad429df2f4f6fbd2f29cd4dc0d82db180
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    displayName:"Test API",
    targetUrl:"https://someapi.com/api",
    authenticationConfiguration: {
      @odata.type:"#microsoft.graph.basicAuthentication",
      username:"<USERNAME>",
      password:"<PASSWORD>"
    }
};

let res = await client.api('/identity/apiConnectors')
    .version('beta')
    .post(identityApiConnector);

```