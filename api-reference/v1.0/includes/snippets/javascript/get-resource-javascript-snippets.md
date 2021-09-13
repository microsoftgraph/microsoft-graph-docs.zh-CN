---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b84e7455b64488fe5aacf13e6ad3cc449ea80984c02860604814566943af0f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/onenote/resources/{id}/content')
    .get();

```