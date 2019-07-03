---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 843df898cb71b1baff3466fbe308060490d6c548
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/UsedRange')
    .version('beta')
    .get();

```