---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d02168d063dfa18571c53298a1dd822dd90e93ad012629f71df888075797f98b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237058"
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