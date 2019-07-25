---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e1a831ebd8112eefce0339186006abb9087a8a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const publishedResource = {
    displayName: "Demo provisioning (updated)"
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d')
    .version('beta')
    .update({publishedResource : publishedResource});

```