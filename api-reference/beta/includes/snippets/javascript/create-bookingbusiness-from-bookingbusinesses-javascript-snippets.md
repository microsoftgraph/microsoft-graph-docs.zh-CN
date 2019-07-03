---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b30d372de18860269bde1849a7a9f3f01d2abb3f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingBusiness = {
    displayName:"Fourth Coffee",
    address:{
        type:"mall",
        postOfficeBox:"P.O. Box 123",
        street:"4567 Main Street",
        city:"Buffalo",
        state:"NY",
        countryOrRegion:"USA",
        postalCode:"98052"
    },
    phone:"206-555-0100",
    email:"manager@fourthcoffee.com",
    webSiteUrl:"https://www.fourthcoffee.com",
    defaultCurrencyIso:"USD"
};

let res = await client.api('/bookingBusinesses')
    .version('beta')
    .post({bookingBusiness : bookingBusiness});

```