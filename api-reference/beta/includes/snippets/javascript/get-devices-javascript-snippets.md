---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f01abeaeb4f046c033526ad8737b291a4ee1c2df
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500667"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices')
    .version('beta')
    .get();

```