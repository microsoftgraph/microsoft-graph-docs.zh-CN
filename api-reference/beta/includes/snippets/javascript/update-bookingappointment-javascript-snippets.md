---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bd603b1c57fdad30d46906aa8246b630d8da278e4ad51b6342cda62879ae36f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingAppointment = {
    '@odata.type':'#microsoft.graph.bookingAppointment',
    end: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-06T12:30:00.0000000+00:00',
        timeZone: 'UTC'
    },
    invoiceDate: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-06T12:30:00.0000000+00:00',
        timeZone: 'UTC'
    },
    start: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-06T12:00:00.0000000+00:00',
        timeZone: 'UTC'
    }
};

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=')
    .version('beta')
    .update(bookingAppointment);

```