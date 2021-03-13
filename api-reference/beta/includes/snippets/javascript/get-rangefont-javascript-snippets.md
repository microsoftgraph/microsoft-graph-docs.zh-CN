---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4108bc33540f7a591b9c92c4bc0512e3d1a80f9a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFont = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/font')
    .version('beta')
    .get();

```