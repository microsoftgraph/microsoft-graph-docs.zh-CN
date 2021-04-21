---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eb9ca19f2ba18802638a047ec0928f1f9a65b64
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: 'UserFlowWithAPIConnector',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1,
    apiConnectorConfiguration: {
        postFederationSignup: {
            '@odata.id': 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}'
        },
        postAttributeCollection: {
            '@odata.id': 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}'
        }
    }
};

await client.api('/identity/b2xUserFlows')
    .post(b2xIdentityUserFlow);

```