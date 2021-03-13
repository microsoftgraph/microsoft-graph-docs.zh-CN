---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3fa1ee598dbc6838f5d67b51746b654d5ea039a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connector = {
  '@odata.id': 'https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}'
};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref')
    .version('beta')
    .post(connector);

```