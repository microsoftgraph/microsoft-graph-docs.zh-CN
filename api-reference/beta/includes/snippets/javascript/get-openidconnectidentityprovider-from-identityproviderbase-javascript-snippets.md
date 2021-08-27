---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f1c81c4688d805de9a72fed7f4e1525f8e3d0388728e13a1112bad18a3f741e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000')
    .version('beta')
    .get();

```