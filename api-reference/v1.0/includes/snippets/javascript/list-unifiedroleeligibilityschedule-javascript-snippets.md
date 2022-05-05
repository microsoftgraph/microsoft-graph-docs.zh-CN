---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a74047e28a33a9fab2044c96be89f2dc59b8d748
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206940"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleEligibilitySchedules = await client.api('/roleManagement/directory/roleEligibilitySchedules')
    .get();

```