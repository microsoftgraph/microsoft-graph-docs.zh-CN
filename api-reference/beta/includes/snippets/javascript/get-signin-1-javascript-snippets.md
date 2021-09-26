---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc900de0f14dd7926e54db6315ca7cd4043941a6bf2e5471cddde33a62e3962d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIn = await client.api('/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100')
    .version('beta')
    .get();

```