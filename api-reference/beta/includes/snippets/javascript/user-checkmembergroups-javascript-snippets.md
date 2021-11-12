---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88c18962c904b463a2faedbe08e78aa37e439e79db5d869fd11781fe216b62b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106245"
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

await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(string);

```