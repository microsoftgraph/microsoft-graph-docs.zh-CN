---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 98caf7a9baa53c4c152b874b8d1e91c7ed2f483f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455854"
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