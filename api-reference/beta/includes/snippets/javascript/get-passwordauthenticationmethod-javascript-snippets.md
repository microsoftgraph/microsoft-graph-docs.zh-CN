---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43d1cc1a9c34a2868a5fb77e877e851c80f339a6c6c5d8cbef4a73ea7c89e739
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordAuthenticationMethod = await client.api('/me/authentication/passwordMethods/{id}')
    .version('beta')
    .get();

```