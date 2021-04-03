---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bebd9cf3d1f4f800939a1ffafc2dbe923a0b29a0
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506929"
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