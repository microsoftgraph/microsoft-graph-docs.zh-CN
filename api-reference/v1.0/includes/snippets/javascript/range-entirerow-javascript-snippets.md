---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00debe751e0766f3f740f300fe9ed796f6665520
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/entireRow')
    .get();

```