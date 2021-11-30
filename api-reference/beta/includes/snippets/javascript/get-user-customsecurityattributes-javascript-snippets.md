---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8e1f1b9d452185c8b76c528a12d93b45d45163f
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/users/{id}')
    .version('beta')
    .select('customSecurityAttributes')
    .get();

```