---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec486bd858f11011496061ec7e2a13b74909cfb2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequest = await client.api('/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .filter('userConsentRequests/any(u:u/status eq \'InProgress\')')
    .get();

```