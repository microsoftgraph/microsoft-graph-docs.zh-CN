---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14bd3556319512eb5fd925ec990ffee6e256a01ac2a27f90c7878eb75c6c1f9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220667"
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