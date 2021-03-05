---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1648d030dc5b0a478bbb1f532b4842990b199321
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq \'876df28f-2e78-423b-94a5-44181bd0e225\'')
    .expand('appDefinitions')
    .get();

```