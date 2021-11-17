---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68677e53ab15fcc33e5206e3377c43308dd5897cd01b03d07c8b05d46bf2e9f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sets = await client.api('/termStore/groups/{groupId}/sets')
    .version('beta')
    .get();

```