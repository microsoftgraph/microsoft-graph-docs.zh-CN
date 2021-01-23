---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0e1fedec7347efee890f4751f5e8248053a6e33
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9')
    .version('beta')
    .get();

```