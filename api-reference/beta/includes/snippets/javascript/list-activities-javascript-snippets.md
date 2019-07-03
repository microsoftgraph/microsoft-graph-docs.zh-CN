---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5cec1d6afdf41b96655384e3ac370b761f3648c3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/activities')
    .version('beta')
    .get();

```