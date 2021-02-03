---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f643f77e8118da985dd2342eeb2a83bd0d26db4
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{id}/assignmentSettings')
    .version('beta')
    .get();

```