---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4179d1c50bd257ab60854e59746f37855760822f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/me/tasks/lists')
    .version('beta')
    .get();

```