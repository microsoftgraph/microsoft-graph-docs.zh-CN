---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7a82f4d96c34054cf575fb5eed6e8f08b3bd049
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873205"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/AAMkADIyAAAAABrJAAA=')
    .version('beta')
    .get();

```