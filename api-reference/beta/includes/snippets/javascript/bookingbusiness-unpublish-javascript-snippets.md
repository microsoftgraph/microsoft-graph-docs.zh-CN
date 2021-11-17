---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffb4d95c1ae9612e6637fba00fef969c4911af088ef1cffa9777ef241f8d50ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish')
    .version('beta')
    .post();

```