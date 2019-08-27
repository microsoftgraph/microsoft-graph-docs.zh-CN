---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82a037f42f9ec2de8af543ab0738170a922a962b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/14008"
};

let res = await client.api('/education/schools/{id}/users/$ref')
    .version('beta')
    .post(educationUser);

```