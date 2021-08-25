---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3da501b26bc51ad2497b6b18132804952319ffd370486a72a7cd17540fdbeba2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/{id}/conversations/{id}/threads')
    .version('beta')
    .get();

```