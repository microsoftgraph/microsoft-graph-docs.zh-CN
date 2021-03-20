---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 095878df1758182099e0383c0025953fd06d2346
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945757"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/drive/items/{id}/workbook/names')
    .version('beta')
    .get();

```