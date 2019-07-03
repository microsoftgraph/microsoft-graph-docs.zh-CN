---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ee1b3d58344dff6b0108e885aa98128f08b5c554
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)')
    .post();

```