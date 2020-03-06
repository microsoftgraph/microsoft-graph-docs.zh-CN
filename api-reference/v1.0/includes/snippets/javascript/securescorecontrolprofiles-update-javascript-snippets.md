---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4262ea3ba91bf7b1f1be0f9d15fb5772ef3a0d19
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const secureScoreControlProfile = {
  assignedTo: "",
  comment: "control is reviewed",
  state: "Reviewed",
  vendorInformation: {
    provider: "SecureScore",
    providerVersion: null,
    subProvider: null,
    vendor: "Microsoft"
  }
};

let res = await client.api('/security/secureScoreControlProfiles/NonOwnerAccess')
    .update(secureScoreControlProfile);

```