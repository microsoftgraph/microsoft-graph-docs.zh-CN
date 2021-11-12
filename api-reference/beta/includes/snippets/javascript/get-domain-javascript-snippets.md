---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b70903a816827e4944e077cb90197545c92e78abfd50db1d005fad7774f7e494
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domain = await client.api('/domains/contoso.com')
    .version('beta')
    .get();

```