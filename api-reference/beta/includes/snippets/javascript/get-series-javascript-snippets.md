---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a27d5b8bafa8b4a244babb58e57fb3a8165a6ed0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let series = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .version('beta')
    .get();

```