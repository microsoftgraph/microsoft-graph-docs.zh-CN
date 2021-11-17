---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3edc339a81b3580e948f48147f1e5a74ec840ba
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let device = await client.api('/devices/6a59ea83-02bd-468f-a40b-f2c3d1821983')
    .version('beta')
    .select('id,extensionAttributes')
    .get();

```