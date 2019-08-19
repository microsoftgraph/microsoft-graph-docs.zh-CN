---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0938d06e5416becca7574fbee25f4faa115ca246
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/analytics/settings')
    .version('beta')
    .get();

```