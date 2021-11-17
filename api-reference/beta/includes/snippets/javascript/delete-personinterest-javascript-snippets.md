---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9163cb9f03bd7c49a6a70e5a10ac09483d64e0b9bcae645fc65fd9ff869c913
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218907"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/interests/{id}')
    .version('beta')
    .delete();

```