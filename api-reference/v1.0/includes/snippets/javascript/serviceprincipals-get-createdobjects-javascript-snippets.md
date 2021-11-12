---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 523a6539b6c7745238c7cbe67560859efa1fdc9d1c19369651533caa10b5d25a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902457"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let createdObjects = await client.api('/servicePrincipals/{id}/createdObjects')
    .get();

```