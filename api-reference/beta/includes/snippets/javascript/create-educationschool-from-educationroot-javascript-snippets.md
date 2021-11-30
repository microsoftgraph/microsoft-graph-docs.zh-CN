---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9886654ab401385001ec6ba3d140c6a1ac787300
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: 'Fabrikam High School',
  description: 'Magnate school for the arts. Los Angeles School District',
  externalSource: 'String',
  principalEmail: 'AmyR@fabrikam.com',
  principalName: 'Amy Roebuck',
  externalPrincipalId: '14007',
  highestGrade: '12',
  lowestGrade: '9',
  schoolNumber: '10002',
  address: {
    city: 'Los Angeles',
    countryOrRegion: 'United States',
    postalCode: '98055',
    state: 'CA',
    street: '12345 Main St.'
  },
  externalId: '10002',
  phone: '+1 (253) 555-0102',
};

await client.api('/education/schools')
    .version('beta')
    .post(educationSchool);

```