---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cb248bd577ecff827ac2d2bc8d766ae72d917d2a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders')
    .version('beta')
    .get();

```