---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8e2b23f1d64e3e0e5efedb1eab04fa0918ccbedd4d88b888c3f7588c1c6be24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewScheduleDefinition = await client.api('/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730')
    .get();

```