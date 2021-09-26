---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41bb3fca0f5eba101ccf99801d075b88981b524a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59765678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let device = await client.api('/devices/000005c3-b7a6-4c61-89fc-80bf5ccfc366')
    .version('beta')
    .get();

```