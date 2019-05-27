---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c2d6a8b800a287437fc0be6b8cb29628c9620a0b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/content')
    .get();

```