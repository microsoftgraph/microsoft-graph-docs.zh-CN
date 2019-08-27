---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 914132138d61a0b361674e99c07a90ec888092e3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: "Dion Matheson",
  givenName: "Dion",
  middleName: null,
  surname: "Matheson",
  mail: "DionM@contoso.com",
  mobilePhone: "+1 (253) 555-0101",
  createdBy: {
    user: {
      displayName: "Susana Rocha",
      id: "14012"
    }
  },
  externalSource: "sis",
  mailingAddress: {
    city: "Los Angeles",
    countryOrRegion: "United States",
    postalCode: "98055",
    state: "CA",
    street: "12345 Main St."
  },
  primaryRole: "student",
  residenceAddress: {
    city: "Los Angeles",
    countryOrRegion: "United States",
    postalCode: "98055",
    state: "CA",
    street: "12345 Main St."
  }
};

let res = await client.api('/education/users')
    .version('beta')
    .post(educationUser);

```