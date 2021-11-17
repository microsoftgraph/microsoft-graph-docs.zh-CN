---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85e5d1e038f23d1cbcdb88c3c790346e0f8f4f7ef82b0cd68b143114c8ed546f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/userFlowAttributes/{id}')
    .version('beta')
    .delete();

```