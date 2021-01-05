---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78bc0fc1cbdfd2b18a84d45cddc4b5bb13865697
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq '876df28f-2e78-423b-94a5-44181bd0e225',')
    .expand('appDefinitions')
    .get();

```