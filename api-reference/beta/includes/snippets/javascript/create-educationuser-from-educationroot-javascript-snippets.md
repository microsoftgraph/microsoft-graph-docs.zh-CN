---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f95614236e97dc5d35d9eaf0558de09df07feaf3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712612"
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
    .post({educationUser : educationUser});

```