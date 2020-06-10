---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 401259dcd257eee64c8636c3292fb10059423f7a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  name: "name-value",
  region: "region-value"
};

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}')
    .version('beta')
    .update(connectorGroup);

```