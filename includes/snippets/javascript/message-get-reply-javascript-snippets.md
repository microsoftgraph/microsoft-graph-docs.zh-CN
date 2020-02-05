---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d451256fee035122fd09bac02a85e8591979adcb
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADI4oeRpAABf0HJUAAA=')
    .get();

```