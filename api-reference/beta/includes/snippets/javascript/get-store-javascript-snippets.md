---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc0507378700f97974ca13bbc627860c37615e3b
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let store = await client.api('/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore')
    .version('beta')
    .get();

```