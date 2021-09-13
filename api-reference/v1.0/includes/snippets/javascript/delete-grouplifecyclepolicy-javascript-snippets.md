---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e064f82f42a3967b04622178dd2df04faaaabe7de5d1041c6ba590fbecce9029
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groupLifecyclePolicies/{id}')
    .delete();

```