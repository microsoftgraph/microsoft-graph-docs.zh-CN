---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3aacc207f08eb89683828a3a25f6ab1919b76d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesPublishingProfile = await client.api('/onPremisesPublishingProfiles/provisioning')
    .version('beta')
    .expand('agentGroups')
    .get();

```