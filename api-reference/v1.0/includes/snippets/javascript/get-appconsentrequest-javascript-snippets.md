---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72a66717fe0f7989abd4784b76bece6adb39c8bf8bb6e2c7a76e27e8e6c7c2ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequest = await client.api('/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed')
    .get();

```