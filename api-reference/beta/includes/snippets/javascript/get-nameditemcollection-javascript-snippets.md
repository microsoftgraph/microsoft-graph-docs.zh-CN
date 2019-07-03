---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c9cbe6db01effef60ab73a6e0c7775017bf822a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names')
    .version('beta')
    .get();

```