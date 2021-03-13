---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e8d9c93341724743bca88b04f3cfe7d1dff93ea
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttribute = {
  description: 'Your new hobby'
};

await client.api('/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby')
    .version('beta')
    .update(identityUserFlowAttribute);

```