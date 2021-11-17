---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e96eebbf972cdc7ef90ae5bd95e3d0d95d7d615427edfac7541633d4ceb2bab7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workPosition = {
  detail: {
    company: {
      displayName: 'Adventureworks Ltd.',
      department: 'Consulting',
      officeLocation: 'AW23/344',
      address: {
        type: 'business',
        street: '123 Patriachy Ponds',
        city: 'Moscow',
        countryOrRegion: 'Russian Federation',
        postalCode: 'RU-34621'
      },
      webUrl: 'https://www.adventureworks.com'
    },
    jobTitle: 'Senior Product Branding Manager II',
    role: 'consulting'
  },
  isCurrent: true
};

await client.api('/me/profile/positions')
    .version('beta')
    .post(workPosition);

```