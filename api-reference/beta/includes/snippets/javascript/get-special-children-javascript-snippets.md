---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 241ace6c3b38993bd1e0ad0448fe75e728eeda48
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/special/{name}/children')
    .version('beta')
    .get();

```