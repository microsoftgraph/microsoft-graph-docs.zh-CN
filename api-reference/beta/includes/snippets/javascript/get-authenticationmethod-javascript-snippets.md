---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e88c9b1331542fce489693eca470cd7a594c76b6
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805743"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/methods/{id}')
    .version('beta')
    .get();

```