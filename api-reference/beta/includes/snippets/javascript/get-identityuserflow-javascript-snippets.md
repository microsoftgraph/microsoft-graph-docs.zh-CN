---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1fd32207f97cbe34dd4fe80560a50ba77097fbc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlow = await client.api('/identity/userFlows/B2C_1_Pol1')
    .version('beta')
    .get();

```