---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6777e4f3f0e7a19bd43f828c844240674f53ac5
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508252"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')')
    .filter('userConsentRequests/any(u:u/status eq \'InProgress\')')
    .get();

```