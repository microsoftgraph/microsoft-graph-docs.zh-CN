---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2e75fbccd83d459e2bf21209c081723e6d5f30d
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "48373298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: "Contoso IWA App",
  signInAudience:"AzureADMyOrg"
};

let res = await client.api('/applications')
    .version('beta')
    .post(application);

```