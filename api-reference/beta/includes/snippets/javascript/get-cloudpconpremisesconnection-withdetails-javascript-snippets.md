---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 592581756e770339236b768e81577472fd90dd16
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}')
    .version('beta')
    .select('id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse')
    .get();

```