---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7a2e8bf119d147b425afdeafecb57f6f098850f
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7')
    .version('beta')
    .delete();

```