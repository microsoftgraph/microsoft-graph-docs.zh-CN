---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 441ca65350ce2a7294c1989a738add2e372f3ffa
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

let res = await client.api('/contacts/{id}/getMemberGroups')
    .post(string);

```