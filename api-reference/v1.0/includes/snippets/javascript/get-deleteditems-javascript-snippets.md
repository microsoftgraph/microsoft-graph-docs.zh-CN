---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67d9cf882a18b6c29c1a3884d66b8ff6f42bca41
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/directory/deletedItems/microsoft.graph.group')
    .get();

```