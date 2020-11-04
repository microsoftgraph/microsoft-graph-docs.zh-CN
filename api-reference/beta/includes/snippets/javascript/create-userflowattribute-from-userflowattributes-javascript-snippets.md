---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95ddfd7f12ae9a6f9d2eea455ce6b12d69533ef0
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttribute = {
  displayName: "Hobby",
  description: "Your hobby",
  dataType: "string",
};

let res = await client.api('/identity/userFlowAttributes')
    .version('beta')
    .post(identityUserFlowAttribute);

```