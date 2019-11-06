---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92708c0884c1c9434e8460d2eefbcedc513a5b01
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationalActivity = {
  completionMonthYear: "datetime-value",
  endMonthYear: "datetime-value",
  institution: {
    description: "description-value",
    displayName: "displayName-value",
    location: {
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
  program: {
    abbreviation: "abbreviation-value",
    activities: "activities-value",
    awards: "awards-value",
    description: "description-value",
    displayName: "displayName-value",
    fieldsOfStudy: "fieldsOfStudy-value",
    grade: "grade-value",
    notes: "notes-value",
    webUrl: "webUrl-value"
  },
  startMonthYear: "datetime-value"
};

let res = await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .update(educationalActivity);

```