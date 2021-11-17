---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93b0fc1cf3ca3ee50b594bd6600e8ce5b4c2d1322ec258f6dae17d7ef734b3c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .filter(' (status eq \'Completed\')')
    .get();

```