---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 000ec8a4b2def31bca0f2a2e1db00474c703dc44
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let publishedResources = await client.api('/onPremisesPublishingProfiles/{publishingType}/publishedResources')
    .version('beta')
    .expand('agentGroups')
    .get();

```