---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5061f9c03ebd5bdc927ba706a92ec456d300eab9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomer = {
    displayName: 'Joni Sherman',
    emailAddress: 'jonis@relecloud.com',
    addresses: [
        {
            postOfficeBox: '',
            street: '4567 Main Street',
            city: 'Buffalo',
            state: 'NY',
            countryOrRegion: 'USA',
            postalCode: '98052',
            type: 'home'
        },
        {
            postOfficeBox: '',
            street: '4570 Main Street',
            city: 'Buffalo',
            state: 'NY',
            countryOrRegion: 'USA',
            postalCode: '98054',
            type: 'business'
        }
    ],
    phones: [
        {
            number: '206-555-0100',
            type: 'home'
        },
        {
            number: '206-555-0200',
            type: 'business'
        }
     ]
};

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customers')
    .version('beta')
    .post(bookingCustomer);

```