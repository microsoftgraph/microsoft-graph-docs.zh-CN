---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 393ff8c2813fb849fc5e967a4c084ea3e6ac7584
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drives')
    .get();

```