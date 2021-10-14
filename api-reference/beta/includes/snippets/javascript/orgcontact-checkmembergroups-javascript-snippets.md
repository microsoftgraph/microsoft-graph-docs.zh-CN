---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fe44a29b3f640f93f444d0a46e2393da70a55aee6c4e18893f732a2871fa2f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903508"
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

await client.api('/contacts/{id}/checkMemberGroups')
    .version('beta')
    .post(string);

```