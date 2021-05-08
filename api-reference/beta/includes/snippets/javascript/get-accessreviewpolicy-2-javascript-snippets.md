---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd66e1680196cb26017651e871964472c79807ef
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240991"
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