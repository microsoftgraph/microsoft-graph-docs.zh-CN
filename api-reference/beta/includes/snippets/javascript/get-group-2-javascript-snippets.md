---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ba555704798629df7eb0110a5d3b7f039f59e9c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/termStore/groups')
    .version('beta')
    .get();

```