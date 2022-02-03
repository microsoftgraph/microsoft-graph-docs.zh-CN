---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3f76386b85570f13b7350cd6695d4cbad7f15eb
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61523655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/cloudPCs/ff4eb6ab-d56a-4edf-90c1-baaec8dd6032/troubleshoot')
    .version('beta')
    .post();

```