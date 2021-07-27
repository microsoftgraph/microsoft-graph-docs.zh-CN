---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54e2396cea42dd573076b6cb796f579c7824b057
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C')
    .version('beta')
    .get();

```