---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00db367cccc06f7d9e8670176f88bbc5ddf05261
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/transitiveMemberOf')
    .version('beta')
    .get();

```