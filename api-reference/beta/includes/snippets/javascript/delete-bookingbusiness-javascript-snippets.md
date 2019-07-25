---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e61a974cb61955c2806809212eb9506133fd8f46
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com')
    .version('beta')
    .delete();

```