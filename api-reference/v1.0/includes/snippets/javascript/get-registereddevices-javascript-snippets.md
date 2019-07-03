---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5aa7e87dae7ac7a2449ad08bc7cab97ad1dc1d3d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/registeredDevices')
    .get();

```