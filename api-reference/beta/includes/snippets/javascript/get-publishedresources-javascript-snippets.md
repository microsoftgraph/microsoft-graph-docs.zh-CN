---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f26a10698ceab5f758ba60d65e1196938747cc0b63a78420ed3da8bd4e7bf4d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278023"
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