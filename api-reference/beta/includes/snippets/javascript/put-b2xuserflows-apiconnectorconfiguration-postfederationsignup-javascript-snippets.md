---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a3ab13089b60bab24b87e83406aa34d11bb3034
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843825"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    @odata.id: "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
};

let res = await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref')
    .version('beta')
    .put(identityApiConnector);

```