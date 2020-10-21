---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f3b60f6d3d9a5f3eff155a3b3589f1a6f8bb9d3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastRow')
    .get();

```