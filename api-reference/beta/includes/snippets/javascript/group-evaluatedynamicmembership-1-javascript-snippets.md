---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7b68310b139c5e32a0f6125d4677bad39d70f9e511941efb759fb7b4291a595
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const evaluateDynamicMembershipResult = {
  memberId: '319b41e8-d9e4-42f8-bdc9-741113f48b33'
};

await client.api('/groups/{id}/evaluateDynamicMembership')
    .version('beta')
    .post(evaluateDynamicMembershipResult);

```