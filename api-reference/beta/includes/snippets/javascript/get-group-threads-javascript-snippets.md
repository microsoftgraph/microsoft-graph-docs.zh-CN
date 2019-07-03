---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cfeab76fee4f086cc4dd5759c4b487418905349c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads')
    .version('beta')
    .get();

```