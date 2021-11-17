---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d61b33c2e018110f779161123b38729cf570c02f28200620f4a639e6840535f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104055"
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