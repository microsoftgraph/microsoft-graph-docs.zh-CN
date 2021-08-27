---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3347aaac1f11b491188b20613900dff005d596f3f6cea72a3a185966a075774a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/Amazon-OAUTH')
    .version('beta')
    .get();

```