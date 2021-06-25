---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff609730030f88f13936cc7b70d1d9797645df22
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIn = await client.api('/auditLogs/signIns/66ea54eb-6301-4ee5-be62-ff5a759b0100')
    .get();

```