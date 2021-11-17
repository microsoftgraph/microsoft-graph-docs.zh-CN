---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c67cb49752a2228e5d1ab30299049bac60cff7739345bec9d0961060b2da2143
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/b2xUserFlows/{id}/identityProviders')
    .version('beta')
    .get();

```