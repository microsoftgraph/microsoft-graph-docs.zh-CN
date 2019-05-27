---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5b984fdbab25d82743d6fc43ff2a22a895d067e7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465613"
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
    .update({bookingAppointment : bookingAppointment});

```