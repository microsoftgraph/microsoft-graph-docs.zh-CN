---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19fb5aa3779794a7c6656afb0cdba34994a35ace
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736647"
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

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers')
    .version('beta')
    .post(bookingCustomer);

```