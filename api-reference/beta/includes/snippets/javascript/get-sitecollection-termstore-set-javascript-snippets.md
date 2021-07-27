---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3dc3c59e545e12bc1c084bb245df4e87748bbe6
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let set = await client.api('/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f')
    .version('beta')
    .get();

```