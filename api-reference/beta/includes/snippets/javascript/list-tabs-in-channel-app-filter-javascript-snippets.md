---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f7b0b27d7a0aad7c7f7810dabc6e6d502f8756b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs')
    .version('beta')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.planner\'')
    .expand('teamsApp')
    .get();

```