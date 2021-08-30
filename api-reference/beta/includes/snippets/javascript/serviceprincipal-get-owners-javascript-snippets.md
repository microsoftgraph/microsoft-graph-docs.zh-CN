---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5353c69d87fd32c8ae50d83aeca8f23e9bfe94dd65cc453a7f42f2a1e4d426c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278363"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/servicePrincipals/{id}/owners')
    .version('beta')
    .get();

```