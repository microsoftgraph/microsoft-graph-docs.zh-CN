---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 35aff41c8d3b1223ed8f5716714a9bd4e1570d8d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716075"
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