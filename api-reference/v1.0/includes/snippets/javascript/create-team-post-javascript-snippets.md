---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42fb61f2aa6bd9d4c089fce06407b6ba65084157
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "48315291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  displayName: "My Sample Team",
  description: "My Sample Team’s Description"
};

let res = await client.api('/teams')
    .post(team);

```