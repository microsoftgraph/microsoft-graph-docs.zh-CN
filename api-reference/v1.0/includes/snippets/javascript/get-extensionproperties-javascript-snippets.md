---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe605816ba285fc296ae1fef570dbc817277f28d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extensionProperties = await client.api('/applications/{id}/extensionProperties')
    .get();

```