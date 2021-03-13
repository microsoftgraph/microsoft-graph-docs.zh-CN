---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54b4afe0875aa377e303e46278360dd324817171
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs')
    .version('beta')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.planner\'')
    .expand('teamsApp')
    .get();

```