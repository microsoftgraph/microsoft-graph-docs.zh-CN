---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1036124b2ed5127aa19f4a8433ebb6261cafe3c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let joinedTeams = await client.api('/me/joinedTeams')
    .version('beta')
    .get();

```