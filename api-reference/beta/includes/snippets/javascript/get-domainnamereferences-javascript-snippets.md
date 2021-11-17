---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c74b6a56358cf275734b3b58d374401e43e4e646916eedd1fee90896a089f9db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domainNameReferences = await client.api('/domains/contoso.com/domainNameReferences')
    .version('beta')
    .get();

```