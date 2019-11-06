---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aef4f25c096dce39bfd5f940737b446f8066e86
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const projectParticipation = {
  categories: [
    "categories-value"
  ],
  client: {
    displayName: "displayName-value",
    pronunciation: "pronunciation-value",
    department: "department-value",
    officeLocation: "officeLocation-value",
    address: {
      type: "type-value",
      postOfficeBox: "postOfficeBox-value",
      street: "street-value",
      city: "city-value",
      state: "state-value",
      countryOrRegion: "countryOrRegion-value",
      postalCode: "postalCode-value"
    },
    webUrl: "webUrl-value"
  },
  displayName: "displayName-value",
  detail: {
    company: {
      displayName: "displayName-value",
      pronunciation: "pronunciation-value",
      department: "department-value",
      officeLocation: "officeLocation-value",
      address: {
        type: "type-value",
        postOfficeBox: "postOfficeBox-value",
        street: "street-value",
        city: "city-value",
        state: "state-value",
        countryOrRegion: "countryOrRegion-value",
        postalCode: "postalCode-value"
      },
      webUrl: "webUrl-value"
    },
    description: "description-value",
    endMonthYear: "datetime-value",
    jobTitle: "jobTitle-value",
    role: "role-value",
    startMonthYear: "datetime-value",
    summary: "summary-value"
  },
  colleagues: [
    {
      displayName: "displayName-value",
      relationship: "relationship-value",
      userPrincipalName: "userPrincipalName-value"
    }
  ],
  sponsors: [
    {
      displayName: "displayName-value",
      relationship: "relationship-value",
      userPrincipalName: "userPrincipalName-value"
    }
  ]
};

let res = await client.api('/me/profile/projects/{id}')
    .version('beta')
    .update(projectParticipation);

```