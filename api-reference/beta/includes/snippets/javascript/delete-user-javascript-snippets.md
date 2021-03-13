---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63ee9df694e32844561792853d217a59b01b8fcc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4')
    .version('beta')
    .delete();

```