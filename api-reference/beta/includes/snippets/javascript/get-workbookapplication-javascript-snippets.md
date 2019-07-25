---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f8cb1f2e23b095557abd15ad53fd4d6e1506aa78
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/application')
    .version('beta')
    .get();

```