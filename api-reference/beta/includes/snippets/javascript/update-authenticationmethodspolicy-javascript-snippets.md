---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a3d82244dfccff51b5f3710b233c136476b4379b764d54aa39ce550fb2af43f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodsPolicy = {
  registrationEnforcement: {
    authenticationMethodsRegistrationCampaign: {
        snoozeDurationInDays: 1,
        state: 'enabled',
        excludeTargets: [],
        includeTargets: [
            {
                id: '3ee3a9de-0a86-4e12-a287-9769accf1ba2',
                targetType: 'group',
                targetedAuthenticationMethod: 'microsoftAuthenticator'
            }
        ]
    }
  }
};

await client.api('/policies/authenticationMethodsPolicy')
    .version('beta')
    .update(authenticationMethodsPolicy);

```