---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b6e698719810a2bbbc934f51bd3840f6929ee63
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/cloudPCs')
    .version('beta')
    .get();

```