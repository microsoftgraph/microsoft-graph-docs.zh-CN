---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f319bd661f206e92b71e0c6322c42cdbf3c936dfea62cd5db28e9d1a2a62f015
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334009"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const adminConsentRequestPolicy = {
  isEnabled: true,
  notifyReviewers: true,
  remindersEnabled: true,
  requestDurationInDays: 5,
  reviewers: [
    {
      query: '/users/b6879be8-fb87-4482-a72e-18445d2b5c54',
      queryType: 'MicrosoftGraph'
    },
    {
      query: '/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9',
      queryType: 'MicrosoftGraph'
    }
  ]
};

await client.api('/policies/adminConsentRequestPolicy')
    .put(adminConsentRequestPolicy);

```