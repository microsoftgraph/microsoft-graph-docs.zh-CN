---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 913a565c4e5c17ff4bc784e203ea05f2579eb03a9bdf47a6ebcaedc749ba1e92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220597"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let securityAction = await client.api('/security/securityActions/{id}')
    .version('beta')
    .get();

```