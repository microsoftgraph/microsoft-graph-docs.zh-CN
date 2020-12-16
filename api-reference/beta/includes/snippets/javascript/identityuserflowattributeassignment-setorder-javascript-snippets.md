---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad921da28860c7871f8ca53c1a21ca9e465d8c4c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689191"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setOrder = Content-Type: application/json
Content-length: 90

{
  newAssignmentOrder: {
    order: [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
};

let res = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder')
    .version('beta')
    .post(setOrder);

```