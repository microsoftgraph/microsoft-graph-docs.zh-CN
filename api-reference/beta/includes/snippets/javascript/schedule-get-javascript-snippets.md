---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a933bca14391cde78dffff9175fbd631f3a4d75a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799507"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedule = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .get();

```