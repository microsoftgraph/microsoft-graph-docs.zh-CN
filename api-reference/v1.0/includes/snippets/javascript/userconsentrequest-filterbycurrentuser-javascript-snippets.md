---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c5cac0b8379da2349ed58324098b05cd4609787a7fd6e6740285e16bc0af7a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')')
    .filter(' (status eq \'Completed\')')
    .get();

```