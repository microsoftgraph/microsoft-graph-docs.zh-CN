---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f89b425cc7ae023e0fb42f0605e5639509d511839c70732083fae38d2fe2e20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105240"
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