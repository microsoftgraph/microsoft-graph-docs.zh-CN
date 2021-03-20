---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8df862d5a55a974785a81599aff366aad0e7e6af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961861"
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