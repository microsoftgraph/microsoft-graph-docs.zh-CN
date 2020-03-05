---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 290fa32df7d0e559dfc26b61f46ee612b0ce9762
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997843"
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

let res = await client.api('/me/profile/educationalActivities')
    .version('beta')
    .post(educationalActivity);

```