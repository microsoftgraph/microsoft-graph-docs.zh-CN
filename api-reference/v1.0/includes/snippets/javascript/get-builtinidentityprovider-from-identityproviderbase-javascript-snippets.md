---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4d26bb8640f16acf79bbc8f10b62c9db8ea8bd7
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/MSASignup-OAUTH')
    .get();

```