---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bce612492cd8847c1fcb32d5387f8e9e8b12ed1f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationalActivity = {
  completionMonthYear: "Date",
  endMonthYear: "Date",
  institution: {
    description: null,
    displayName: "Colorado State University",
    location: {
      type: "business",
      postOfficeBox: null,
      street: "12000 E Prospect Rd",
      city: "Fort Collins",
      state: "Colorado",
      countryOrRegion: "USA",
      postalCode: "80525"
    },
    webUrl: "https://www.colostate.edu"
  },
  program: {
    abbreviation: "MBA",
    activities: null,
    awards: null,
    description: "Master of Business Administration with a major in Entreprenuership and Finance.",
    displayName: "Master of Business Administration",
    fieldsOfStudy: null,
    grade: "3.9",
    notes: null,
    webUrl: "https://biz.colostate.edu"
  },
  startMonthYear: "Date"
};

let res = await client.api('/me/profile/educationalActivities')
    .version('beta')
    .post(educationalActivity);

```