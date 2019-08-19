---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b31cc05f77b88c74839bbe735da20557d11fdb25
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/attachments')
    .version('beta')
    .get();

```