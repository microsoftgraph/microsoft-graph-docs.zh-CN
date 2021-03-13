---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd6eb7eff3cc339851960c7df7e5a0b167df8310
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/97a5a533-833d-494b-b543-c0afe026cb96/teamwork/installedApps')
    .version('beta')
    .filter('teamsApp/externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .expand('teamsAppDefinition')
    .get();

```