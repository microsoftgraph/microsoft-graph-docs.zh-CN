---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 795424fbd0c29691ddbe668837d36bf7369329ea
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIn = await client.api('/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100')
    .version('beta')
    .get();

```