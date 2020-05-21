---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01fb0a91ac79405b985d6da88d0ee2992e8e5452
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  displayName: "My Class Team",
  description: "My Class Team’s Description"
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```