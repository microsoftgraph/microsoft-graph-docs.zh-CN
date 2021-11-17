---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30feffc2f2331391ee84ddedcb454e1e87d098bb0c5b18481ec1d350a7a1d25f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  action: 'alert',
  activityGroupNames: [],
  confidence: 0,
  description: 'This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.',
  expirationDateTime: '2019-03-01T21:43:37.5031462+00:00',
  externalId: 'Test--8586509942679764298MS501',
  fileHashType: 'sha256',
  fileHashValue: 'aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313',
  killChain: [],
  malwareFamilyNames: [],
  severity: 0,
  tags: [],
  targetProduct: 'Azure Sentinel',
  threatType: 'WatchList',
  tlpLevel: 'green'
};

await client.api('/security/tiIndicators')
    .version('beta')
    .post(tiIndicator);

```