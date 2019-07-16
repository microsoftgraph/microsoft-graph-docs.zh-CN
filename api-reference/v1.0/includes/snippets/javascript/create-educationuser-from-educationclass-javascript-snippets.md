---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a46abe6071333cfafc15bdc21ae625cc5b965a31
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/v1.0/education/users/14011"
};

let res = await client.api('/education/classes/{class-id}/teachers/$ref')
    .post({educationUser : educationUser});

```