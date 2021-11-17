---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 001d0533b55b296f8d554767a9fd7dcebdacd0ef2afa07c370c50828883962ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequest = await client.api('/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed')
    .version('beta')
    .get();

```