---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50b2756e91f85a9938511d3876e0884d438efeac7e994eefb0f1d7a2fa1c2f09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userConsentRequest = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/acef2660-d194-4943-b927-4fe4fb5cb7e3')
    .version('beta')
    .get();

```