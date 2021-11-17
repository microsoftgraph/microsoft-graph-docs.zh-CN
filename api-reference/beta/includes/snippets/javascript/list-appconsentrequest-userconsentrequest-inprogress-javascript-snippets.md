---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fc3e1bab3174d8f19c154b1b15f91d8cc185d1b67e449696d0b5e9823e9e76a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests')
    .version('beta')
    .filter('userConsentRequests/any (u:u/status eq \'InProgress\')')
    .get();

```