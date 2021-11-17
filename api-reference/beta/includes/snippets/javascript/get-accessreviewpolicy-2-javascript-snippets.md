---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63f1a05361b3f9662b3175227b9532c93789c0f8325364d1ca444adf16afd943
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewPolicy = await client.api('/identityGovernance/accessReviews/policy')
    .version('beta')
    .get();

```