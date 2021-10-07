---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa6d155a550c750dd17671f7d75d1b24dfbfbd7176cc1acbf46742ce6fc017b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq \'876df28f-2e78-423b-94a5-44181bd0e225\'')
    .expand('appDefinitions')
    .get();

```