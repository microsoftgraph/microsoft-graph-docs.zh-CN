---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6fad1ad1cebe3c5f13cb694603e03ab8d3672bb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .filter('userConsentRequests/any(u:u/status eq \'InProgress\')')
    .get();

```