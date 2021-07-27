---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4ac4ddb923b63684e5582c5d9a4613abd4a8cae
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schema = await client.api('/connections/contosohr/schema')
    .get();

```