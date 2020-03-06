---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ffba2550baaf37d56a0352e5650e81527c642be
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636863"
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
    .post(educationUser);

```