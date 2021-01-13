---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4435f40324cd8dc21102962ddb245f476b9b8260
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/apiConnectors')
    .version('beta')
    .get();

```