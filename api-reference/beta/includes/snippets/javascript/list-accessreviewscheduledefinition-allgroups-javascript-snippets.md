---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fa67eaaccd4d21cf85a4a9464f809b8e786d188
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let definitions = await client.api('/identityGovernance/accessReviews/definitions')
    .version('beta')
    .filter('contains(scope/microsoft.graph.accessReviewQueryScope/query, \'./members\')')
    .get();

```