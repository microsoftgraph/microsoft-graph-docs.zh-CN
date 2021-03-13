---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0371185cf7e275ffd254cc24592fdc39e6cff11c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printerShares/{id}/allowedUsers/{id}/$ref')
    .version('beta')
    .delete();

```