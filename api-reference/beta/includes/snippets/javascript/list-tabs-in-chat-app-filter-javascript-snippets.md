---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2a100d3bf3ba37b56966af65cff926116457500
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775799"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.web\'')
    .expand('teamsApp')
    .get();

```