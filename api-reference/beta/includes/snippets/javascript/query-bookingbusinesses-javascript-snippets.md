---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab079ebba1ba27dbc4ee676611008327d114a9a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingBusinesses = await client.api('/bookingBusinesses?query=Adventure')
    .version('beta')
    .get();

```