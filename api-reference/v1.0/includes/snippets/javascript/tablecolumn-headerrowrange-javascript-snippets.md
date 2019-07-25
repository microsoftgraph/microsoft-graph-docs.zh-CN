---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bfa2c2d22552b22cf9d9fa93ff696725e35ba6e9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/headerRowRange')
    .post();

```