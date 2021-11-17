---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13734d29131b1cdc6c6919803e58aa74ab3105333b0dcba93ce2438f84139bb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewInstanceDecisionItem = await client.api('/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06')
    .version('beta')
    .get();

```