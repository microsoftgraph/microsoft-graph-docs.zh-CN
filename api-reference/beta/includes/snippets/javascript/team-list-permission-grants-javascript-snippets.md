---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55abb5d66f194490928402d5adcf176ac644b0e4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrants = await client.api('/teams/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants')
    .version('beta')
    .get();

```