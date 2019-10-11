---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04457f89adf27585f436da4d53592a11291bd667
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  groupId: "ffffffff-ffff-ffff-ffff-ffffffffffff"
};

let res = await client.api('/groupLifecyclePolicies/renewGroup')
    .version('beta')
    .post(_boolean);

```