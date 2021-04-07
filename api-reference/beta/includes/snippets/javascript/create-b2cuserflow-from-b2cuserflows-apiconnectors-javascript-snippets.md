---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 096fff2981e38b3f675d0d1edcea6b3edf0bbccb
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51613503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
    id: 'UserFlowWithAPIConnector',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1,
    apiConnectorConfiguration: {
        postFederationSignup: {
            '@odata.id': '{apiConnectorId}'
        },
        postAttributeCollection: {
            '@odata.id': '{apiConnectorId}'
        }
    }
};

await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```