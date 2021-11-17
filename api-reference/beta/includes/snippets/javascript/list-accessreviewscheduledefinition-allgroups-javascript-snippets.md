---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a6c89f0881595fb6b18d26d5888a748c4dd5af353f72483b39a32d346c4fd2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902625"
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