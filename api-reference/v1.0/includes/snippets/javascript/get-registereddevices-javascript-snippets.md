---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5aa7e87dae7ac7a2449ad08bc7cab97ad1dc1d3d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/registeredDevices')
    .get();

```