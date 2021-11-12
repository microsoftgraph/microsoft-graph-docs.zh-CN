---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab65716fadc1278672dbc512adec3816ba83c9e8cd6dd92c31f39bcf3281a151
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    'groupIds-value'
  ]
};

await client.api('/groups/{id}/checkMemberGroups')
    .version('beta')
    .post(string);

```