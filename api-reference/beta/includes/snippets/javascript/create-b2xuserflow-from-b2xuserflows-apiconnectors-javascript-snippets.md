---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8bc16180ea4225ece7e18b1c8063036602112a6
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49844377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: "UserFlowWithAPIConnector",
    userFlowType: "signUpOrSignIn",
    userFlowTypeVersion: 1,
    apiConnectorConfiguration:{
        postFederationSignup:{
            @odata.id: "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        },
        postAttributeCollection:{
            @odata.id: "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        }
    }
};

let res = await client.api('/identity/b2xUserFlows')
    .version('beta')
    .post(b2xIdentityUserFlow);

```