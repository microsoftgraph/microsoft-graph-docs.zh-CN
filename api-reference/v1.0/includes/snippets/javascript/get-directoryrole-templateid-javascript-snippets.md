---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30aa79af9cba0780310cb034b6f65d7fed312f5e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf')
    .get();

```