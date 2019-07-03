---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c57ae5d1231c2c9c6a867c6a286e91afe410b674
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=')
    .version('beta')
    .get();

```