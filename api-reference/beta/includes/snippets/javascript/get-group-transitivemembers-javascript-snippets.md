---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9047375d83ae19df1c66bf2e052b357ff665e3c0c965c96b982b9fa82981216
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMembers = await client.api('/groups/{id}/transitiveMembers')
    .version('beta')
    .get();

```