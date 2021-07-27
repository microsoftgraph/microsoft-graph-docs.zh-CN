---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f256a82a7773bb44908f570d53fefaa0ee681fb2
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579880"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/connections/contosohr/items/TSP228082938')
    .delete();

```