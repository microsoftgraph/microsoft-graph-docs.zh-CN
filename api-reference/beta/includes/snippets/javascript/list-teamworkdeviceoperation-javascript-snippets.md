---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 403962bc0187a2c41c9f1c1f2fa51c0248bddfbb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations')
    .version('beta')
    .get();

```