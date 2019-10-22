---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 334da94eb53e080a948d278eaaf2070e0aedb895
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "37553956"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: "Fabrikam High School",
  description: "Magnate school for the arts. Los Angeles School District",
  status: "String",
  externalSource: "String",
  principalEmail: "AmyR@fabrikam.com",
  principalName: "Amy Roebuck",
  externalPrincipalId: "14007",
  highestGrade: "12",
  lowestGrade: "9",
  schoolNumber: "10002",
  address: {
    city: "Los Angeles",
    countryOrRegion: "United States",
    postalCode: "98055",
    state: "CA",
    street: "12345 Main St."
  },
  externalId: "10002",
  phone: "+1 (253) 555-0102",
};

let res = await client.api('/education/schools')
    .post(educationSchool);

```