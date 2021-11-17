---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0df162b6c18b13fc30516d55558cd2099b0159bf3113c9bb6c8000eef5a36244
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttribute = await client.api('/identity/userFlowAttributes/{id}')
    .version('beta')
    .get();

```