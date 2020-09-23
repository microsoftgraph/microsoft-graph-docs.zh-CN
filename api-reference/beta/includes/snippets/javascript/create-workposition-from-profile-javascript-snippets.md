---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43f87240af5cca11eaa958e2c5f152f66f0b9c70
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workPosition = {
  detail: {
    company: {
      displayName: "Adventureworks Ltd.",
      department: "Consulting",
      officeLocation: "AW23/344",
      address: {
        type: "business",
        street: "123 Patriachy Ponds",
        city: "Moscow",
        countryOrRegion: "Russian Federation",
        postalCode: "RU-34621"
      },
      webUrl: "https://www.adventureworks.com"
    },
    jobTitle: "Senior Product Branding Manager II",
    role: "consulting"
  },
  isCurrent: true
};

let res = await client.api('/me/profile/positions')
    .version('beta')
    .post(workPosition);

```