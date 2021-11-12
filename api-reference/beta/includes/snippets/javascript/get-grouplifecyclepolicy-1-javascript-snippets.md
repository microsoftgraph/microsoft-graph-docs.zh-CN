---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47394c6682997bfbea961812f19816f9366bc1ed27a8bcaccb09076abafd778f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicy = await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .get();

```