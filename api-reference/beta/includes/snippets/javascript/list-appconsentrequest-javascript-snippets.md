---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e28fdbd3bb35685125a03fd76b916d3dd7f4112922abd5acf2b1b147f74cf558
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests')
    .version('beta')
    .get();

```