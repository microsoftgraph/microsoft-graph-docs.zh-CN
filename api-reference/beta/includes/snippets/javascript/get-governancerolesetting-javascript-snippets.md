---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d85fe652c7075847ef2ed487e0ed055e3cb8baf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let governanceRoleSetting = await client.api('/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9')
    .version('beta')
    .get();

```