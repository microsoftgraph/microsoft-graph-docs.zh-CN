---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b201d36ad4e5895ee3bb54b7a3b95ac5f6c14453
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll')
    .post();

```