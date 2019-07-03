---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 37a2658d9c4dcb30632ed49d2ac10cc5fd3afbd1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .get();

```