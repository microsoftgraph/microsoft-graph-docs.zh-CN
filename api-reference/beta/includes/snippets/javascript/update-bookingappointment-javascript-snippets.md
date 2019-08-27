---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2731f21834a4ac088a42290a5435b3cfc9465dca
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingAppointment = {
    @odata.type:"#microsoft.graph.bookingAppointment",
    end:{
        @odata.type:"#microsoft.graph.dateTimeTimeZone",
        dateTime:"2018-05-06T12:30:00.0000000+00:00",
        timeZone:"UTC"
    },
    invoiceDate:{
        @odata.type:"#microsoft.graph.dateTimeTimeZone",
        dateTime:"2018-05-06T12:30:00.0000000+00:00",
        timeZone:"UTC"
    },
    start:{
        @odata.type:"#microsoft.graph.dateTimeTimeZone",
        dateTime:"2018-05-06T12:00:00.0000000+00:00",
        timeZone:"UTC"
    }
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=')
    .version('beta')
    .update(bookingAppointment);

```