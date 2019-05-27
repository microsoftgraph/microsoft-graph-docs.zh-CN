---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e092ecffd01da1a5f95dc10b99d4a75e3d663e90
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453802"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/usedRange')
    .get();

```