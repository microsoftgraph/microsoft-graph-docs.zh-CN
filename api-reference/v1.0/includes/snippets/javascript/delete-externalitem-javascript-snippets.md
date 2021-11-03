---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36d888174820876f8aeeef4136904cfaad5e0ff3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/items/TSP228082938')
    .delete();

```