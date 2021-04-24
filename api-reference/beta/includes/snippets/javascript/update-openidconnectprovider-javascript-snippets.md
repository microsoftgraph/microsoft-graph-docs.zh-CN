---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01a360dddbabaf26e84a307d1fdb0459c4be726f
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51987540"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  responseType: 'id_token'
};

await client.api('/identityProviders/OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a')
    .version('beta')
    .update(identityProvider);

```