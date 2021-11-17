---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3064b987130e5d1bc65b6acfef4ed7588cd31187ac98897877b286e88069873a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let phoneAuthenticationMethod = await client.api('/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7')
    .version('beta')
    .get();

```