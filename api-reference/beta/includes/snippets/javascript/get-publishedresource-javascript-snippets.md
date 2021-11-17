---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 091c948f2678a0cb11f0290371ea1ead19519d91c3cfd18a3be1a9a079d9ac9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163085"
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