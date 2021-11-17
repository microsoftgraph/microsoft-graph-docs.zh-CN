---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47f5a86f5ddec55f4d5b0312e53151852daf20c38bd7891d03179234042a4e62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesAgent = await client.api('/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/')
    .version('beta')
    .expand('agentGroups')
    .get();

```