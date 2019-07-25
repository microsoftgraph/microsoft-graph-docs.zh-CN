---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 15603d9b0b9926480d4d54f7977ec0de2814e529
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)')
    .version('beta')
    .post();

```