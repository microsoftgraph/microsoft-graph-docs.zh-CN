---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f892f6ad39452f04694b6264926317b65b26b7d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingBusiness = {
    displayName: 'Fourth Coffee',
    address: {
        type: 'mall',
        postOfficeBox: 'P.O. Box 123',
        street: '4567 Main Street',
        city: 'Buffalo',
        state: 'NY',
        countryOrRegion: 'USA',
        postalCode: '98052'
    },
    phone: '206-555-0100',
    email: 'manager@fourthcoffee.com',
    webSiteUrl: 'https://www.fourthcoffee.com',
    defaultCurrencyIso: 'USD'
};

await client.api('/bookingBusinesses')
    .version('beta')
    .post(bookingBusiness);

```