---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 963662a959ef37341b6333e8c992d7f2ff8a79ad
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/me/getMemberGroups')
    .version('beta')
    .post(String);

```