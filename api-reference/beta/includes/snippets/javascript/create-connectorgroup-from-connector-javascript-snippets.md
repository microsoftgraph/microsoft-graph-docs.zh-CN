---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe2a78a6af7993a63d930904916e01fd27f43549
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  @odata.id: "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"
};

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref')
    .version('beta')
    .post(connectorGroup);

```