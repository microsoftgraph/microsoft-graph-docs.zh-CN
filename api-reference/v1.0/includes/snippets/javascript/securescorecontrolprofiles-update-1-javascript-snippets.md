---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bc0841fca52ef5bae49896c7a38ed82aa63959340c15dee63b0082721b194e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const secureScoreControlProfile = {
  assignedTo: '',
  comment: 'control is reviewed',
  state: 'Reviewed',
  vendorInformation: {

    provider: 'SecureScore',
    providerVersion: null,
    subProvider: null,
    vendor: 'Microsoft'
  }
};

await client.api('/security/secureScoreControlProfiles/NonOwnerAccess')
    .update(secureScoreControlProfile);

```