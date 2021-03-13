---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dc1e09aaab7232decca913b764f690549c50931
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppInstallation = await client.api('/teams/{id}/installedApps/{id}')
    .version('beta')
    .expand('teamsAppDefinition')
    .get();

```