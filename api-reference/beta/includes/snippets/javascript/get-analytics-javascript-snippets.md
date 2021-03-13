---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe275d3f20b5f6607c9ad77545ba7561eadc281d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemAnalytics = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .version('beta')
    .get();

```