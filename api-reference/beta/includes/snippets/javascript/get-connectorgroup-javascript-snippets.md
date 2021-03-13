---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2681ce16ad54ec6e24c9c28c0b427333e05e3fc4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801229"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectorGroup = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}')
    .version('beta')
    .get();

```