---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a62bdee83fc055b00409be70aac20fcf6be8603affed9fb778eb8753f4dc45a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332509"
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