---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ed70107120ac4e41b6581a3994291fa88e6c5c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications')
    .version('beta')
    .get();

```