---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da709ed6f9cd0b27c5f6fa9622fb07611e063b6d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationalActivity = {
  institution: {
    location: {
      type: 'business',
      postOfficeBox: null,
      street: '12000 E Prospect Rd',
      city: 'Fort Collins',
      state: 'Colorado',
      countryOrRegion: 'USA',
      postalCode: '80525'
    }
  }
};

await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .update(educationalActivity);

```