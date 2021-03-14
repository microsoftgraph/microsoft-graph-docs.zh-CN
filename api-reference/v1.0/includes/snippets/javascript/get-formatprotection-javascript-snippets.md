---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5350892c114cc13dc3ada8afd56121cee2d65c1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookFormatProtection = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/protection')
    .get();

```