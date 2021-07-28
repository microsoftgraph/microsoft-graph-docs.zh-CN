---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d383e557d49c5788c51e5ed3a705a1aac220746
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalConnection = await client.api('/connections/contosohr')
    .get();

```