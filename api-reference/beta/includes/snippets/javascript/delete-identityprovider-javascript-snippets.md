---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05f9dfbc3e04ddf3bfa9c0c22dd910e1560a3b24
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/Amazon-OAuth')
    .version('beta')
    .delete();

```