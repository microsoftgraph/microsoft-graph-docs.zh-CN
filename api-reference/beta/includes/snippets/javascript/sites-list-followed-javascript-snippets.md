---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7a44ca17c394d879c7813c0fcc70846a6c7f1a4
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/followedSites')
    .version('beta')
    .get();

```