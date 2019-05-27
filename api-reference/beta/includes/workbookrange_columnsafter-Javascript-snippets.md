---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 35aff41c8d3b1223ed8f5716714a9bd4e1570d8d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)')
    .version('beta')
    .post();

```