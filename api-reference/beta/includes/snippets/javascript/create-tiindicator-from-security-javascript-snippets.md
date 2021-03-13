---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa6bd73586315ed100e6623ebb31a43a4aabbe13
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797040"
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