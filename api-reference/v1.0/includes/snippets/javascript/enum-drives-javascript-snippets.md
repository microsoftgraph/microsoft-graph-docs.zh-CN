---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 393ff8c2813fb849fc5e967a4c084ea3e6ac7584
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drives')
    .get();

```