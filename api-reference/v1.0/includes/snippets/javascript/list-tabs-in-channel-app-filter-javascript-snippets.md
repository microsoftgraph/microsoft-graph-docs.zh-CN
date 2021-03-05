---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a807f4d3c81c43b1f8b60c8f326788cc2d87ac17
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.planner\'')
    .expand('teamsApp')
    .get();

```