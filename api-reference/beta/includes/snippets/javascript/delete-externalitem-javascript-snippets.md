---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 218b8f82d825ec8de2699e3c9b498c759475c356
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .delete();

```