---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe1ff095065ddbbf76c37024d8817091a034959a
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "48315294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  displayName: "My Sample Team",
  description: "My Sample Team’s Description",
  owners@odata.bind: [
    "https://graph.microsoft.com/v1.0/users('userId')"
  ]
};

let res = await client.api('/teams')
    .post(team);

```