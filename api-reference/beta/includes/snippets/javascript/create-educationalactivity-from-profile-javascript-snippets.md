---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91a8fa7cece43d95aba2882ca4dd561ee61c7dc81fe4ba1e4b0f83693b6d1fb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationalActivity = {
  completionMonthYear: 'Date',
  endMonthYear: 'Date',
  institution: {
    description: null,
    displayName: 'Colorado State University',
    location: {
      type: 'business',
      postOfficeBox: null,
      street: '12000 E Prospect Rd',
      city: 'Fort Collins',
      state: 'Colorado',
      countryOrRegion: 'USA',
      postalCode: '80525'
    },
    webUrl: 'https://www.colostate.edu'
  },
  program: {
    abbreviation: 'MBA',
    activities: null,
    awards: null,
    description: 'Master of Business Administration with a major in Entreprenuership and Finance.',
    displayName: 'Master of Business Administration',
    fieldsOfStudy: null,
    grade: '3.9',
    notes: null,
    webUrl: 'https://biz.colostate.edu'
  },
  startMonthYear: 'Date'
};

await client.api('/me/profile/educationalActivities')
    .version('beta')
    .post(educationalActivity);

```