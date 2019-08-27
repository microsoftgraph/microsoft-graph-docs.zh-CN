---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bbe6926eee21b3d87f75805f63a81327237f756f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636582"
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
    .post(bookingBusiness);

```