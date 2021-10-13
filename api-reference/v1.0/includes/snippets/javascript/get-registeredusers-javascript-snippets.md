---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 956001d158e5e01c534c044e3ade2dac5521826e5eb15555ae28910df3af68aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredUsers = await client.api('/devices/{id}/registeredUsers')
    .get();

```