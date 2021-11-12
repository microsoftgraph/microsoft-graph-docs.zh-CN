---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcc39c313d496fe2ed9520ad516b2bad0afa1e9807a01f98397085f46b1143ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273899"
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