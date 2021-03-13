---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b59df0b0cbf4f3066eb6d735bf630e48b58723f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: 'Fabrikam High School',
  description: 'Magnate school for the arts. Los Angeles School District',
  status: 'String',
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