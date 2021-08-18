---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0bfacd092cd969cd4d8359a19c54944561a289e79f259c26d8fde8a93c6e4e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162482"
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