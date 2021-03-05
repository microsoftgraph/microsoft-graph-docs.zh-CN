---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffa2be12558ca35b5ca343cd338228a25a4930ab
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq \'b1c5353a-7aca-41b3-830f-27d5218fe0e5\'')
    .get();

```