---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95d82d8bb9f3677c8813dd46f6d3aa1d6847b855
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear')
    .version('beta')
    .post();

```