---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44af917de6f1ef022afad514a1411314dc4f2733
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const evaluateDynamicMembershipResult = {
  memberId: "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  membershipRule: "(user.displayName -startsWith \"EndTestUser\")"
};

let res = await client.api('/groups/evaluateDynamicMembership')
    .version('beta')
    .post(evaluateDynamicMembershipResult);

```