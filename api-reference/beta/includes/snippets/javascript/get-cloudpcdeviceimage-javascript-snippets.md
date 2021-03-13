---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 551504d5314615e9c96016e8d715f9287349ca90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcDeviceImage = await client.api('/deviceManagement/virtualEndpoint/deviceImages/{id}')
    .version('beta')
    .get();

```