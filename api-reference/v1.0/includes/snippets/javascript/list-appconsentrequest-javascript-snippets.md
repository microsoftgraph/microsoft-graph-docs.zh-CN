---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1504d92e0ad0af3a1135f94311531c8783ec3329a0db4d176efa49cf638ad77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333276"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests')
    .get();

```