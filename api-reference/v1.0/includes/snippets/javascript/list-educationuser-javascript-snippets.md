---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3dbcb9b7adbdca32524eaa47771e578378d4cbddd9839383a52b6c7f42f8590
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/users')
    .get();

```