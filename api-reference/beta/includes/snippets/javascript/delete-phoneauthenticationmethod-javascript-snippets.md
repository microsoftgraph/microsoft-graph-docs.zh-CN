---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9688aa87f8142da3a5670aff472f1188d54b65dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7')
    .version('beta')
    .delete();

```