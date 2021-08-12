---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8367444af942537b16dba7c0eb3fa618617d01b6d92ddc12485f7bc889fbeb78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADI4oeRpAABf0HJUAAA=')
    .get();

```