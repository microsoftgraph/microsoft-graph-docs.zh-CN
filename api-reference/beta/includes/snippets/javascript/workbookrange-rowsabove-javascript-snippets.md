---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15603d9b0b9926480d4d54f7977ec0de2814e529
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607000"
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