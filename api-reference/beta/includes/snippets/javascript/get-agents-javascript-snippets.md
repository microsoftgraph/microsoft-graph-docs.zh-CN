---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc3dc910495d378b85a9ba6b3b7cb6130923addc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agents = await client.api('/onPremisesPublishingProfiles/provisioning/agents')
    .version('beta')
    .expand('agentGroups')
    .get();

```