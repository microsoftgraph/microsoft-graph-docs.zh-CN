---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f26f92e176716b102972cb9aa4d6704e95e6bbf
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewStage = await client.api('/identityGovernance/accessReviews/definitions/6af553ce-104d-4842-ab5f-67d7b556e9dd/instances/9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24/stages/839ecbd4-ba5d-4d32-8249-e734aac47adf')
    .version('beta')
    .get();

```