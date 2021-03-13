---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a568c2e38efba1c54f5c06a1785030fc51524a3b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
  isLanguageCustomizationEnabled: true,
  defaultLanguageTag: 'en',
};

await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp')
    .version('beta')
    .update(b2cIdentityUserFlow);

```