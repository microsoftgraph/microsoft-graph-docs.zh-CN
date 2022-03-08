---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2849f6ff6836db073d035c0aa956bc2280f0be59
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesPublishingProfile = await client.api('/onPremisesPublishingProfiles/provisioning')
    .version('beta')
    .expand('publishedResources,agents,agentGroups')
    .get();

```