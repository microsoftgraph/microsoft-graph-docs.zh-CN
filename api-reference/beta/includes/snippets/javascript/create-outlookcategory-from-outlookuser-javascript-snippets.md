---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b0fc7a9bf547c377b98abccbb37868205d2a1d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName: 'Project expenses',
      color: 'preset9'
};

await client.api('/me/outlook/masterCategories')
    .version('beta')
    .post(outlookCategory);

```