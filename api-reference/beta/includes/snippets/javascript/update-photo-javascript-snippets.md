---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8322c3da19c7c81745947ef69e03ae2ebe38dce9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profilePhoto = {
  height: 99,
  width: 99,
  id: "id-value"
};

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .version('beta')
    .update({profilePhoto : profilePhoto});

```