---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8360322445e20eec99d5cdb1919a6c220472220d
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49844216"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
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

let res = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```