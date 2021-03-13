---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9fe72754e6fe1342c162323b4a6af67b9806786
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781551"
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