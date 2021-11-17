---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a79bd0a7a154ac6b5b593755e191c72fa43837682a047898d8a4edbf5517d597
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328866"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/plans/{id}')
    .version('beta')
    .delete();

```