---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39231c353010b704a7849999452114f7f8c2e135437ed4c4bb9f040974dad02d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220748"
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