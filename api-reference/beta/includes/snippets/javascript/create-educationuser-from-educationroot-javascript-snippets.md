---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 290d4c705c6cff62568b57886bdad04a4f4b95c26f2dbecf238e95e6f51caf4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105779"
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