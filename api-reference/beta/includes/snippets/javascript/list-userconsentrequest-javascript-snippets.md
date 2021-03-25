---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d4a4dff85d476196a335a78b6201649c24d7586
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests')
    .version('beta')
    .get();

```