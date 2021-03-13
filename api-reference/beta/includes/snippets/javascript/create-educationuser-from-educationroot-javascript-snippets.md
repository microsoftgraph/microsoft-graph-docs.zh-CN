---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84d8fbb9933d8fd429e94a6d1fa0f022376c6643
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: 'Dion Matheson',
  givenName: 'Dion',
  middleName: null,
  surname: 'Matheson',
  mail: 'DionM@contoso.com',
  mobilePhone: '+1 (253) 555-0101',
  createdBy: {
    user: {
      displayName: 'Susana Rocha',
      id: '14012'
    }
  },
  externalSource: 'sis',
  mailingAddress: {
    city: 'Los Angeles',
    countryOrRegion: 'United States',
    postalCode: '98055',
    state: 'CA',
    street: '12345 Main St.'
  },
  primaryRole: 'student',
  residenceAddress: {
    city: 'Los Angeles',
    countryOrRegion: 'United States',
    postalCode: '98055',
    state: 'CA',
    street: '12345 Main St.'
  }
};

await client.api('/education/users')
    .version('beta')
    .post(educationUser);

```