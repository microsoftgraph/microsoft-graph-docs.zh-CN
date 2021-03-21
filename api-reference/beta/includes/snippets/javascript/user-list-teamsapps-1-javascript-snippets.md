---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1498d1990e16e68ccd6b08b55fd22321c44809b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userScopeTeamsAppInstallation = await client.api('/users/{id}/teamwork/installedApps/{id}')
    .version('beta')
    .get();

```