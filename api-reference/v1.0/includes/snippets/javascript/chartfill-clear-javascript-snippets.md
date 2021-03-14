---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 715ed95757f10efe1d3f0b8cc6fdc3e569bd04a1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear')
    .post();

```