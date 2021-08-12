---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7dd00bb3d31da9f21ac033649cf27e7fb0a6772c064f341ef289b83b3ba5703
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=')
    .version('beta')
    .get();

```