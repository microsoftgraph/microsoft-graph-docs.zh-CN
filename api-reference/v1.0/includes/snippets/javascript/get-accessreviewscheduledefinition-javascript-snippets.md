---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a56c826ac28bb5979f321b6bc6b0bbc1a8bbe9e7
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewScheduleDefinition = await client.api('/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730')
    .get();

```