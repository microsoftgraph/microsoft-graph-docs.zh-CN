---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55ffd376706cf33f9b52dd24ddf056023773669f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869081"
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