---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f747518f80a5209a97413f0e1a2584cd3074d64
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members')
    .version('beta')
    .get();

```