---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15094f8a9e4606db1854823ee5e99495a5c15898c84ad830444217d538da8779
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902263"
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
    .post(string);

```