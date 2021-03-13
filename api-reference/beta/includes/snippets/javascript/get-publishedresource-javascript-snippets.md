---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbb27fbd71648e03f1639b866bd9643f19925b04
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let publishedResource = await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/')
    .version('beta')
    .expand('agentGroups')
    .get();

```