---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3b39dcbd0c6b6b1702aa1bf5b6792aa85bfda65577e51fc2cc0c2aaf7860d28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alert = await client.api('/security/alerts/{id}')
    .version('beta')
    .get();

```