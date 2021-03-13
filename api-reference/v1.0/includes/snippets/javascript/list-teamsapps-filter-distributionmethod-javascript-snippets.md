---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0de7c9cc842d7c825ed6f02d9e3e97890658418
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .filter('distributionMethod eq \'organization\'')
    .get();

```