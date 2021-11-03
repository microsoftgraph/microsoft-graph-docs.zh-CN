---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e7cb8cf31e690d925dfcbd6a63a851b54d52d94940daf83328eae64fe426824
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingAppointment = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=')
    .version('beta')
    .get();

```