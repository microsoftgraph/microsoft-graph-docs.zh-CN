---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e7d993e40f582f9b2e95f22608d72876d24a8e81
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/attachments')
    .get();

```