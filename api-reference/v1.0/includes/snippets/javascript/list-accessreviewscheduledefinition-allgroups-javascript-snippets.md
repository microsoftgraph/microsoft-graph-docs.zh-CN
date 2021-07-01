---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e01f1a527df4b74049cfcfbc4bfab53ecd53248
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208684"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let definitions = await client.api('/identityGovernance/accessReviews/definitions')
    .filter('contains(scope/microsoft.graph.accessReviewQueryScope/query, \'./members\')')
    .get();

```