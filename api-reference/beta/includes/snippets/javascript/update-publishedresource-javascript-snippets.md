---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95ee3dc32a010dc0ea0d6923abda56d432e4599879769c16176ace16af3079d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218453"
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