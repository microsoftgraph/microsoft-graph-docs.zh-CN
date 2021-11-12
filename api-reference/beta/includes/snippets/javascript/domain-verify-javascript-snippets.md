---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8132d987482fd15c58e4d0cd34825cc25431b03f258b7d9c32e82e10ca8df440
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/contoso.com/verify')
    .version('beta')
    .post();

```