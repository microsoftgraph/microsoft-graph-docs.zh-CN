---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4deae8ae4a8d5edfe888c7e58a5e2c9cf09ca259
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348296"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkDeviceOperation = await client.api('/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations/eab261f8-61f8-eab2-f861-b2eaf861b2ea')
    .version('beta')
    .get();

```