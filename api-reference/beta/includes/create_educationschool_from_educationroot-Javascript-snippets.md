---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a2520a756a15a43491058fc1bfde560e5218550
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480972"
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
  fax: "+1 (253) 555-0101",
  phone: "+1 (253) 555-0102",
};

let res = await client.api('/education/schools')
    .version('beta')
    .post({educationSchool : educationSchool});

```