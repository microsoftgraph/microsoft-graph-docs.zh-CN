---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 956cdf3698bc1158ee1bbcd46991a27c419d8681
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/connections/contosohr')
    .delete();

```