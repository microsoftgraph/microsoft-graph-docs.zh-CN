---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fcfc6b6f0d660256d3764849facd6330d1e498ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/unsubscribe')
    .version('beta')
    .post();

```