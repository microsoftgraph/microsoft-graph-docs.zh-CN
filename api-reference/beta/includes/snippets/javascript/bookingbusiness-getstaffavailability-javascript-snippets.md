---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8c27a57040f5b76897e423fcd6f79327376c919
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getStaffAvailability = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/getStaffAvailability')
    .version('beta')
    .get();

```