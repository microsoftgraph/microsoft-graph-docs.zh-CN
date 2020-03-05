---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30da32183bd7f058babf47ae427afdab6bf8e090
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996495"
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

let res = await client.api('/me/profile/projects')
    .version('beta')
    .post(projectParticipation);

```