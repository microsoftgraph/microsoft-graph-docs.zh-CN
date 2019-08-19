---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e0eb27e29d16a55eb49f357cead51c9d075be79
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/analytics/activitystatistics')
    .version('beta')
    .get();

```