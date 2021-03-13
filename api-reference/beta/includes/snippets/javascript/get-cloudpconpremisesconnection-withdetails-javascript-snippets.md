---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b3160a42649a435421bb61e4d31079bcdbd4420
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785345"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcOnPremisesConnection = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}')
    .version('beta')
    .select('id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse')
    .get();

```