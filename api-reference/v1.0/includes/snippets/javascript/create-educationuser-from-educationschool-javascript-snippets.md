---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8642aafe1d11c8701907706e0376794c4da83f25
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740639"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/v1.0/education/users/14008"
};

let res = await client.api('/education/schools/{id}/users/$ref')
    .post({educationUser : educationUser});

```