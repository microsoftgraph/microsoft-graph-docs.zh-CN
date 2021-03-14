---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90c4b6b2a8ce20e0bb5d5d23aaf6ced7d14809b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let points = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points')
    .get();

```