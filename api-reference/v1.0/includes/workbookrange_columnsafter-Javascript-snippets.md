---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ee1b3d58344dff6b0108e885aa98128f08b5c554
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)')
    .post();

```