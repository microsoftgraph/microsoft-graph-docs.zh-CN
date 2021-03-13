---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 167c89dcc2f4367889df38a3251950ab901adc91
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemAddress = await client.api('/me/profile/addresses/{id}')
    .version('beta')
    .get();

```