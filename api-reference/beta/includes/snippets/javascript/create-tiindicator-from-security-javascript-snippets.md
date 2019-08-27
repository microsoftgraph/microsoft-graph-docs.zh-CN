---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6fbb76f51f197ef2b2dc01c2642b44e81e5e22f4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  action: "alert",
  activityGroupNames: [],
  confidence: 0,
  description: "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  expirationDateTime: "2019-03-01T21:43:37.5031462+00:00",
  externalId: "Test--8586509942679764298MS501",
  fileHashType: "sha256",
  fileHashValue: "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  killChain: [],
  malwareFamilyNames: [],
  severity: 0,
  tags: [],
  targetProduct: "Azure Sentinel",
  threatType: "WatchList",
  tlpLevel: "green"
};

let res = await client.api('/security/tiIndicators')
    .version('beta')
    .post(tiIndicator);

```