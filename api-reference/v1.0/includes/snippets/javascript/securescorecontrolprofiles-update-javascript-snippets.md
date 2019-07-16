---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 98caf7a9baa53c4c152b874b8d1e91c7ed2f483f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735838"
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
    .update({secureScoreControlProfile : secureScoreControlProfile});

```