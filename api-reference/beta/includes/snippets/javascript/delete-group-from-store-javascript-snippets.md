---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a2d1a703bfa92e8f9e89bf0f8a66932027e27059cc95618008382bc6473e423
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/termStore/groups/{groupId}')
    .version('beta')
    .delete();

```