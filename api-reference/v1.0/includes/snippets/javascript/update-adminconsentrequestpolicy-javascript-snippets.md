---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac4c3380cf828627af4cb352890cc407e6fe19ae
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509180"
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