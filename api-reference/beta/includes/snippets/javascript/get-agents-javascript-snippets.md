---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86eceafd26b983209a465f03a762f92942ee05e6b893f52a928a6a86a1e53b51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278044"
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