---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8504b8579eaa8c46876e4040d724df9418b06b10
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings')
    .version('beta')
    .get();

```