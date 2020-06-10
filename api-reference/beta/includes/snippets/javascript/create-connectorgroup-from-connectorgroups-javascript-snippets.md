---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88c8a74c1ee165fb4b4b0b65f68e0dedb2594cb8
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681239"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  name: "name-value",
  isDefault: false
};

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups')
    .version('beta')
    .post(connectorGroup);

```