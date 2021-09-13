---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e5b86edacc598190be72a11f639ac93099a9a0cb8f6e2feca7067f54e18e384
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278701"
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
    .update(identityUserFlowAttribute);

```