---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b2893395be79e6c0c4c7af22e2782f37b8524bb
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .version('beta')
    .get();

```