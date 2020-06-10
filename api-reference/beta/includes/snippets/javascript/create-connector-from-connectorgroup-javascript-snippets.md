---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa199ca6dad53e37e4d995029b7dbccf8b929b16
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connector = {
  @odata.id: "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
};

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref')
    .version('beta')
    .post(connector);

```