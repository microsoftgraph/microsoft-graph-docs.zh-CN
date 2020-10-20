---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efa003c3b51660c0972c7edf16d5c25ea2247416
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/LastRow')
    .version('beta')
    .get();

```