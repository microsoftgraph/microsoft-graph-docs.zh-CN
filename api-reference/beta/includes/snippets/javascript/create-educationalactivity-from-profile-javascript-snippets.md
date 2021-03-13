---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84f6b4274332a0e166919fc1c5fc3ea7507ef7f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800146"
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