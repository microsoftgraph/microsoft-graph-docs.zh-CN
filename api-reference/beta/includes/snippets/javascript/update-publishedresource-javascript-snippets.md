---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c8df312b7f9631c907403197933001a1a65537d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const publishedResource = {
    displayName: 'Demo provisioning (updated)'
};

await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d')
    .version('beta')
    .update(publishedResource);

```