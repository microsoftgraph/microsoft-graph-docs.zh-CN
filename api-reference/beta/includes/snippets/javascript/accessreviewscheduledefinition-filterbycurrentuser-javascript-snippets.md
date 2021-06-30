---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e5e412eb3ee0abf7c034a1243f091de90a62ff1
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .get();

```