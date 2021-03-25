---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 892b39751c8f03e9a1c826ea9c38842b2d45fd60
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userConsentRequest = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .filter(' (status eq \'Completed\')')
    .get();

```