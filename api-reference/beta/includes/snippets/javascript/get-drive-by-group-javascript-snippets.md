---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d9df8c58185550f65c048473b2b262ccc81aace51e6785c65d04ba9213b7666
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/groups/{groupId}/drive')
    .version('beta')
    .get();

```