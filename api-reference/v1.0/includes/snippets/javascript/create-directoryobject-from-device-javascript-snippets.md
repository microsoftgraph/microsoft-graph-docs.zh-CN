---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1639314342eb0edb36b03c0ec085169ce431c8bf
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/devices/{id}/registeredOwners/$ref')
    .post(directoryObject);

```