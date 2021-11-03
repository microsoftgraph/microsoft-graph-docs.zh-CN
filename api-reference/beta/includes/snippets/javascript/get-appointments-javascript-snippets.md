---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc18a234c39e40a79571d4637e3621044775be8669cb0a0757a2de2299c5abb7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appointments = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments')
    .version('beta')
    .get();

```