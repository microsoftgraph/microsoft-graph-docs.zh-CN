---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9d5bc6ac63d6026b701b533891326a38f15f64dcf92912289242e7dd6b2a157
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903145"
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