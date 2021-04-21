---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1e8eac45454a2ea3547bb3dbb04edcac1d7ad5a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921460"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/Apple-Managed-OIDC')
    .version('beta')
    .get();

```