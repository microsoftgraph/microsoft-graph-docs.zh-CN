---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b30f866aae9d418a7af79c09ce11cd5ecd60e66
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range')
    .get();

```