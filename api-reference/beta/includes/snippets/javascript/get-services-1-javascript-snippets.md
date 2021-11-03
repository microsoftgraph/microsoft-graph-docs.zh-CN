---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22c9ce1eedd6449b9dc255f26a85c63f7173df21fb74fa3844d6ad2266ed61ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let services = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services')
    .version('beta')
    .get();

```