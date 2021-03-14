---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a295c3be145b477c84e399cbb72f700af12b662
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFont = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/font')
    .get();

```