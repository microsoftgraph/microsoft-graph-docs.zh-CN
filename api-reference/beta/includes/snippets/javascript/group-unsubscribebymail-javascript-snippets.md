---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1058a230b5951dad2c7473933c17560f5d485626
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/unsubscribeByMail')
    .version('beta')
    .post();

```