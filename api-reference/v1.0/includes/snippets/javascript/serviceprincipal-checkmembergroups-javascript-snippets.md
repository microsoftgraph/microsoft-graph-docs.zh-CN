---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb5ecda21c5bdd7e9c26b3286bc7c2c0795153fe5d1e3dfec73b4250f521cbbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334082"
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

await client.api('/servicePrincipals/{id}/checkMemberGroups')
    .post(string);

```