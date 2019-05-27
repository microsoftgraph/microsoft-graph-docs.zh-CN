---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 73106003169e48e9a41d91dd4dac54222e35bee0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436150"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/permissions')
    .version('beta')
    .get();

```