---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7b3598e7c94b391ad3da3f45fa75754991854ce1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/{publishingType}/publishedResources')
    .version('beta')
    .expand('agentGroups')
    .get();

```