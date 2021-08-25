---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bd32952919cb613d4bdbbe088c82abdf0f61f93
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/getMemberGroups')
    .version('beta')
    .post(string);

```