---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5606de65faa80b33c629ba5c1e6d4e5eb9e9bbc4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewHistoryDefinition = await client.api('/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38')
    .get();

```