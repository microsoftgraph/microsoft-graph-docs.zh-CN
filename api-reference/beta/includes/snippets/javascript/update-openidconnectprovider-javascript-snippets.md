---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 229129393148fc762e765c9dee4e131c0947ec44
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  responseType: "id_token"
};

let res = await client.api('/identityProviders/OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a')
    .version('beta')
    .update(identityProvider);

```