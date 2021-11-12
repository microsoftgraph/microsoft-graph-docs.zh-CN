---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4accb328f1d562b8f7099faa721b3432fd9d206ffa4afd771f51259fbd5cf29e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  '@odata.id': 'https://graph.microsoft.com/beta/groups/{id}'
};

await client.api('/print/shares/{id}/allowedGroups/$ref')
    .version('beta')
    .post(group);

```