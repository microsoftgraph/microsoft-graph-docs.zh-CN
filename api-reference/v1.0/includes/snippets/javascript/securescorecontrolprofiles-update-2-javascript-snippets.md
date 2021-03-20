---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d84a9c2ad3e700dbe9eb04a35ecb97f9daf42d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948750"
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