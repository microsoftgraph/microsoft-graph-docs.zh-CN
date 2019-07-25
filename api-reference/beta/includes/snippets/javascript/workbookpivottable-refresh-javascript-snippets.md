---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 89f0e2a2fe7a622dab0b787d2ecc11fdcfa1a676
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh')
    .version('beta')
    .post();

```