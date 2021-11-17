---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b33285127850ac7f6447152ed57a95766fc3568246320d64957f361df43f516
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewScheduleDefinition = await client.api('/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d')
    .version('beta')
    .get();

```