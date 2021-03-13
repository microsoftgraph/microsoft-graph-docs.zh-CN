---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f7b2a5dc766a36847b3d55fea8dd1377b0d39f1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .filter('id eq \'876df28f-2e78-423b-94a5-44181bd0e225\'')
    .expand('appDefinitions')
    .get();

```